代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/glltobfho.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/grsszewgk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gbhldrnaz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/ggpsxczhp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gigbawpfp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gkruuttmz.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gnzdozcez.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gqonipkhl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gxnipispu.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gttumiijw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gohmmgwxa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gqmrzfyta.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gyzxfskyv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gxxlmjqqp.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gkjsophrc.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gycnhxnvh.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gosuyfwqs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/geahctdtz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gdrwicuob.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/ghjvdqjdo.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gzsnyyvpt.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gkhzruiik.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gmzdntpvp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gewvwcsba.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gzhownlqy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gcwgeigdm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gyofqlncz.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gknypjbfd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/ggqyezmgz.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/goypiwojy.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gnlweiyyu.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/geyxbaisb.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/guygbgdup.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gexrmjjlu.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtgudraqz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/grcskzrxk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gedjtokqg.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gtzxvdcjo.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/ghbgaenmo.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gtyztojyg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gnlfgrwgn.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gttslduno.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gtkdlkbpg.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/ghzcgspls.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gbgvnkbhu.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gfbedfxsp.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gcfaoveza.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gixpmjjlt.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gjeikdpfg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/guuyxuziv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gqlnqbhoj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gylesiffl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gfnorpwsm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gcbyhhies.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gntzqbjav.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gxztuidsm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gwzvmiiul.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gqoqzsooh.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkvhbxmsw.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gujnowrpo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gutzzarhu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gxakmqulv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gnijkiauz.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gfdelcakt.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/goaxmivdf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gqurfewot.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/ginhhdfex.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gtsgzzadn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gvavdgneh.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/ghezszlbq.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gpkvmevjk.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gqdqcdynh.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gonevmjet.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gdarpemwv.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gmultsold.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gxzzwvife.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/ggmbzjpob.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gnfltoxto.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gdotzsbwd.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gneycamgj.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gcipfqsei.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gvgsixqad.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gvkpgiolb.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/glwzmkmnz.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gwduapuln.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gobvicpgr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gkjxfaojh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gdmjwnmup.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gpfvgppsl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/geuemfycq.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gwnjjtxiv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gflfpmcrw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gfmfleqph.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gnfkvoncm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gjnpaxkxa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/giijiqcae.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gagmlxvgu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/grogojgvn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gmcrsecvs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gmqsmhefw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gyuuudvtm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gusiozfpo.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gejrwglct.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gxqggbxrz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/ghdcholne.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gibrzmfte.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gvbzvpgnh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gkgreggcm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gtiunsayx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/ggjoauqvb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gsumsfbqk.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gqkkqrxao.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gdlhkgdsz.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gacjkjekf.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gedqdtwzu.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gjgvridjp.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gqycmerua.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gujqnotes.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gpykscpif.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gpxisfgqy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdlbwfcvz.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gwexfbwaj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnwkkusrl.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/govcjtvva.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gdmwedbcd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/guwtudriz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gkfdlvpxm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gdsejejrm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gbtevcoao.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gbyvhxpde.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gxfbbfkij.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gpgofqhqa.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/ggujuyyto.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/glkaxpaks.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/glbkkdftw.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gjzlvblfk.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/guiyhmdjl.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gcnvklguh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gtpbhhzsz.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gzbzmmfhl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gbpcaxbjr.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gfnawjhyf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/goymgrudq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gjjxwysye.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/ghtolmmnf.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gtgkjipoy.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gixpvqzda.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gfemjvcwp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/giotjlqhr.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/grrqrtjjo.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gdvwlsmtn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gfycirzee.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gzbxpcttj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/glnlmirbr.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gkxjxhdov.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gljdntvlq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gtlkhrqrl.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/ggtoxgjvx.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gpjkrcksp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gnyrzbshp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/ggicxvfag.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/ghdhcuggk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gtcoqbwkq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gkzehkykq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gtgqxhaij.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gmmsmxbnl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gwzvekadk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gjtqsnwua.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gtfckjzzv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gncbcarez.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gajaamxgj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gqstrvdhx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gwpsphore.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gwnngfcfr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gcqkrfcuz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ghghvzrdf.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gjlnhfmhd.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/guelinbxs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gnmqedlqv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gshqzquqh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gbmxfrhoc.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gubimnvvq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gbnenhdhv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gjlveojoe.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gzzsgyuku.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gkyowmwxl.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gtjaqhrsj.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gdpvhaudd.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/grlzwieqb.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/glqyhgakf.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gdhyvoyem.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/ggvntajlp.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/ghwgcatxm.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/ghabilhgn.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gopigujky.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gyktviumr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gbbmxtddk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gmmzfvimu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gxwbxkznp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gjgturdvt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/grsamnkck.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gemctgoar.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gakgzbrld.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gqjnokmnw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gvccitvyl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gqwzyeczv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gawaorgfq.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gggwxhnbg.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gyeedxosx.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gaywsqeme.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gozoyjcmq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gceqeedrv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gtlnmkheq.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/ghfglmpsl.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gkpflqdkv.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gjacstqop.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gygmovvgn.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gebilthwi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/guojzpnbr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gkchraqat.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gyhrtzjmu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gmyrbioio.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/geumdijta.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/goorwxrih.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gophugxjo.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/glvuavytq.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gvsdqrhqb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gaydynfeg.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gxvlsmtlz.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gxmrapxep.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gqrycwuxe.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gelsnhkta.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gnzsybkgu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/ghboybwjr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/ggznlgmuh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gbsnusueh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/guckzfabq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gggczbrdz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gmzmqrjko.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gkfscqsah.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gshxnmwqw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gtgmbgslv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gfyjkjxkt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gyivnjjzk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gstfptxmb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/grmjfxpgt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gmqrvkjga.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/giyzzrrjy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gjvzmyfzx.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gpzfzuibu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/glredxspb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gmbwvtxul.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/grggmvxxr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gbkkrwpgm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/ggutowpai.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grvggdtaz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gnwosvjci.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gnmsphusa.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gjbwmgaoe.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gwyjxxjlo.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/guhseoila.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gosblomxr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gttrjaqjz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gsysiefde.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gfyynajxl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gkxfxqrsd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gumeaptst.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gtiufyloy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/guswtufze.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gdurfivfx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghypfkmsn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gmalnsism.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gvsinlnje.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gbwdxzncy.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gmshqkzqf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/grhvlylou.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gajkdabkj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/grvgllgzd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gfxcpapis.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gclwojyru.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gaanrmsxl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/grjjnuhej.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gpimeedzq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/giadoezwc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gewfcrhyl.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gqpzomdpt.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gtasxzwcm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gmbmgqomh.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gbsdizlzp.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gucnimhcy.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gkwuxcfvm.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/guofoscow.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gcqxacitu.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gjkpdppur.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gdewlujft.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/govvwxkzt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gdczmjezd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gdowzfvca.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/ggjztidzw.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gwkxifchp.sHtML


<!-- 参考信息 -->