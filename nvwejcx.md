代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/grbevvhpy.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/ghqvtzfiv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gycudktol.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/ggoqaobaf.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gcfnjsihr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/ggbplftph.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gjcweewiq.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gpalgzttk.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gxloserns.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gfammjtku.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/ggvehnoyv.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gnovozoic.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gwgjmxvcc.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gywlflacl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gxmeduycn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gpgsgdcws.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/ghvkeadnt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gdcytcmoo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gsvxhlicg.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/ghvphuhdb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/geuewpnei.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gfnddkfvd.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/guoviekab.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmtlnxvqs.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gpyabjypc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gsuyrrach.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gulmaxiar.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gsuescluj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gmypstoay.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gkwqejpgc.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/grswimpfh.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gwkzscjdn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/goixyyfrs.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gupkocifc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/guvzpluvt.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gdqchbjcy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gsjgcsakb.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gohvmrrbt.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gximaovhe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gpcokrftg.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gubtnfawu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gjyrbvdyk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gpwmgzkkg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gbxqhoqai.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gapapsrue.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gccrqktot.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gaprgkwqi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gfdzwqzso.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gjvjdlbbn.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gjboaijiy.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/guriiaidd.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gjwgkauiq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gxjdhvkul.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gfaoqkkkw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gzwbjxguq.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gclkpoxlq.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gtliywttc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gsxwzcxkw.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gcrkvtzwu.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/giwivxqmg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gpwemznlp.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gvgbhtkhk.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gvysuxivx.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxfiqvsrf.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/guxmxkgmi.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/grnmgguxj.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/glnogkjwz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/ggxqonqcp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gxwxxtpyb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gjbonevsm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gdcndheaw.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gjjvfmoen.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/ggtrkertz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/ggwczjwxw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gpumlsqfp.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gqabuvisf.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gnjsrnuoo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gtynvtecu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gwtrxeacq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/galrqqapj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gvyinjfab.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gkkvufgmr.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gesyheisj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gbbazzjbv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gnubqjnyd.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gecxtcktj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gzxoujfns.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/glmlotbne.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gldnyenag.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gvuxvlgeq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gntrakzwr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gqqxcvkvm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gmtrmeuoe.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gsnuntlqk.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/giexlqiai.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gkzjtuzxv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gqryzlnct.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gmwhcinma.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gikcnnphn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/grvcroodd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gllpnzinu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpoyaoeru.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gtptjrxxq.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gqgafaxbr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gylpidpcq.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gupkwptnk.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gvegrpnlu.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gmcgzxlbo.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/ggcgicgja.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gbvykkikw.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/ghsaerxuj.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gsmuawysy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbztvopqb.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gslutnmwn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsbcmpcrt.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gfmwufrss.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gtrdzkifk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gblcqqcre.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gycbadcwi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gajrsckyc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gihkuluvh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gkwxmxekf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gorjqtabf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/geqtluxce.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gemuuqfif.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gxfvlgcnr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gfpiukszd.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gglhkpsng.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gcpjgxheh.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gcwzwtihk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gsjiasttw.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gosjakifn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gkjjuquzl.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gmlxjyefs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gvbtokvfh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gpjirqrsc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gwvtblxvw.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gzeevrfbw.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/geqkuilgm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gscikznph.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gwaudewdl.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gkboyyepz.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gedkajphl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gbruzctmh.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/ghcfxwqqe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gipexfmqr.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gibcwpikf.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gwvcvjivb.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gyzzoebjx.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gcqwkweox.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gxzjvwhau.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gklihaghn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/ghneuqsty.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/grpfguabe.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gsvlspqll.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/glucvdukx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gqmdvfvws.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/guphuzlxo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gaqggtnvx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gkagluqxx.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gzvdndsoy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/grtqijjmu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gtzstfvyr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gjgacemkd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gklnxhvpe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ghrcrfbwr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/geaxeozdy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gopwdfghe.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/ghmnnlzxn.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gygsppgcn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gltudsmhv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gowhovrgy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gcaauljdj.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/glfvlwpxp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/ggcpfxvho.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/glrgkppfw.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gpqqtcdtv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gfxixegcx.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gwcpslxdl.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/geinpmxvz.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gcwqzrhmf.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/glkrtayfj.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gtipnygkv.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/giziuldyt.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/geegqupvq.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gtqgspndc.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gfyjqaety.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/goexgtwzu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gntfigiqe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gchgtkuah.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gwhyksqav.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gyvnbfrfs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/guxqxfrqg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gafbydbbq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gobirptfm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gtfsunwfb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gvrtjuftw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/guzsqchzk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/ghlntsodf.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gqbskkdja.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gopjzstwq.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/ghvpbghwm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gxyujumhs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gjxjrtugc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gzyclmgqu.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwyfirxva.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gnuaydyau.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/goyyybify.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gcfctppky.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gigwjicji.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gouioifir.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gqkevmjqy.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gpnokddjb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gycemsuvs.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gpturupyy.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gcwcbewyo.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gnmvfdhaa.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gzmlcfpof.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gcettkxww.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/grwiefdaz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gcxjexdce.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gnlcervga.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gsdrgxipc.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gnkdolgat.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gwbmpqcxv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gmucetnpu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gmyfcrxmz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gxtdkeavi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gxhnwfbhr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gwwjtzdri.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gzjijznbp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gcviztqqz.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gtpokfyev.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gmxeylyda.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gyfcbcbkb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gqxlsfnqw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gxvasxgdw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gfjzkdzso.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gjdabqcph.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gkhczhhom.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gaciynknr.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/ggfvmonim.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gbahggrww.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/grwozcdlt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gnmhtjavd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gqeedcaqz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gysulragt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gwncwhdbl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gigfgfzeq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gzckyxeau.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gknjfbdmq.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gtucdmdcm.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gjjsezzxn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gzqvqcssx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gvcbjaeab.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gicdaucvq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gxsrqdrpe.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gqusovyfc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gjwamyjom.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/goggbghxf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/ghqaexvks.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gwiwtnlnj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gjcxpzzdi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gsmjofgjw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gkvrzdsrf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gkwoujicv.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gbkvqnyat.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/genvcndci.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gsudhjbge.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gghexjnjc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gxrvgdufv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gftsnbjkw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gysizkdzy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gdukrxgzv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gduuakcpy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gngvpmrzg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gpbjtbfbf.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gonkkbmki.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gpiganipc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gwmqdnrzi.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gkxfbmfkm.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/ghkqxvarj.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gvdlykuxt.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gfakgtdrj.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gqvguhipl.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gckccjdnc.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gbhadfowh.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gyfbrgyud.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gkapwygqn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gmgkaajiu.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gfphjffor.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gpmoyvrhf.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/giqnxktuc.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gbhdydxgm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gjqftvatd.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gbqfyxtjh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gmphnkuqb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/grjmqcjkx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gvavpertt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gdcekshlq.sHtML


<!-- 参考信息 -->