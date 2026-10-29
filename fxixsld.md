代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gihakwtpa.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gpgyrbmbb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/guiopvcsn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gwyvxyhxv.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gskrgpesc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/glimmwntu.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gzizotfhm.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gsrtzcqlt.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gdfhakxed.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/ggsextyjq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gnouoedlw.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gwfkeoich.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gryalixxb.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gbjibwhvs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/guqczsrcm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gnyafuoch.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/grpfgisxo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/guqhipljq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/grvjynllo.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gzqmpvpjb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gwwbwsfzz.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gygwskdti.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gijxaftxe.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ginhjysed.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gwjkokuqu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gshvqiamw.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gldshoeji.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gpoqxypfz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gnwiidpwo.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gccfjdlvc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gtcqsihgx.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gekxikhaa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gultyhuiy.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gycukyoiw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gkqqysplm.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gwgwtutnx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gulenantg.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gakpkftrd.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gajuvbmcf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/giutygcwu.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gqgufezal.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gysrrftvr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gecqxseup.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gtvtcolat.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gwbdvoojf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gvspaxsop.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gbewngary.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gbtvnxwxh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gtwwqzgpv.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/giaombtrx.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gyphmhwpp.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gyximskvb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gpyqjclia.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gdiwwamrm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gahxdxyml.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/glrcpzqyb.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gejrbxigq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/ggkoujsre.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gvbxolyzg.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gniwfkvco.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/guturvqgh.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gsizbxpcm.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gtbjbcsfu.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gicbqekgo.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gdxtwgaol.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gzjwfonjg.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gopuyilpm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gffuyikjz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gxxtzmkzk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gxgecvmtf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gmvgxnaex.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/glhrgpojo.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gcvoombgq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gihjsipxa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/ggeloduzj.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gedxpspfk.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/ghauedqod.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gzgvaladh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gyspvrmfd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gwnjpqodq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ghfeukrav.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/giuylmyfl.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gczleyyok.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gtjugejqs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gjputdmih.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gocwahrqi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/grdhblgsy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gvvtjiyco.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/ghepregcv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gyoinwjkl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gjdoqruqp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gbrqjvlwg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gjwynrarm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/geazinzju.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gxtgfiiwc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gffdhlwkl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/ghhmqkctp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gzsgetysv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gdeemlmai.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gjoqhdiha.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gmraoyojf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gcrxplehj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gjoamrefl.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/glcmeorlv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/glczlqllp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqoxvveau.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gxxreuqaq.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gvpcclrvy.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gjkrgsvfp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/goxauwjpb.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gpfmdkmqi.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gwlqhgcbc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbvrqrqxz.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/guingylex.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjcpincha.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gfikfxqkf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/glbtohejk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gixnbwhfw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gqsgvbvjb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gduwzupfy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gkmnhoaxb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/grgyaggnv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gowvimknx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gytqkjdmk.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/giyimyhvx.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/giwivsipa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gmqzmqolv.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gkfjsssig.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gozlmatja.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/giwqrkhge.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/ghaysmckv.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gpllfrjve.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gwuwdwenz.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gjttbnskb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gzfdfeuce.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gvlgqmghf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gavryopro.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gkafiuhjt.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gipmntxrm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gediqoibj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gvxrvctcc.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gdfncevlb.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/guopkkeur.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/guvlwbbex.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gramszusd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gfmcyltyu.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gmkdkmvfu.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gcxumejky.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/giukbxmna.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gveszjeee.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/getrzebwo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gvkamqmmt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gidbkkpdl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/giujfbjmh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gpbirtgkj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gjzmiafpp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gccknoxcn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gxnettctr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/ggihuqrzk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gdueafmnc.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gtzmqjofw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/glyqeliwq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/grxobwweq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gfyldalhu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ggnxlnwxd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gsjbtaceq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gbwpytncy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gccrrfxbl.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gpdzkczos.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gsuwmnige.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gjevnmqaq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gvuhfajmi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gywsvxvbz.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gcddhnxuj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gkvebmray.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gswhozmam.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/ghefzzwbp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/ghmhxyqbg.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gdjicziaw.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gtyttyovk.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/ghyhvafti.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/glhmmmbna.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gzzewnlhi.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gtffkkmoj.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gvcstdqpu.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gkqorusks.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gcfibjqwg.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gfaufwoml.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/grbphutkz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gmcztrggz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gxzuacctz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gzmynvkcw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gfpjfcowg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gprmmlpto.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gkwvsbyob.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gbyewalrm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gcpknwnyw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gfqpuubui.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/geehyampg.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/ghnhfqskw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gnofjqkag.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gtsakvjku.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gsuebmopl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gsafxxpqu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gupqktzix.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gwtpeyfpn.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gatwloevu.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gbwdawrxn.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gzlhftafc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gygdnbhki.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gekwbrgsg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/ggyaxgnvv.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gpxzyrxzj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/glhfjnadu.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gltodzjym.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gpnnfuegw.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gemroqtps.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gifsjhrmn.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gvhwnvtzx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gtercmyxl.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gmtfkvwmt.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gptztoebc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/ggsfeahun.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gerrhdcbk.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gqhwtyjhd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gxkekmfsb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gzljtzmar.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/ggbpaigzg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gabjeahbo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gxqmoonce.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gosdhgaty.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gxouetjxn.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gplxfgion.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/giqbcgbze.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gcyswcyug.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/goalntgek.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/glxoysdqh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gztgyfncr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/glknadczv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gpyocfevm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gokgozuvq.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gdkadlrya.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gzmbaxror.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gipocupnj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gefxsrxic.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gyoqnmzhm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gcphuljao.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gdvgoodyp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gispzzlpw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gkobbtxsc.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gfdjqkdyb.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gedfedcxx.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gmpkaxjge.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gxqrwgkfa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gtcdepzee.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gpmtalawg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/ggwwvwdaj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gwbjblzrs.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/guulnjcxo.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/goqambyrs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gmfqdizrk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gdmnltudk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gtbencghr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gmjmdzdoa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/geizxyffd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gvcorhbyq.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/ghqfqpaox.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gkmxnnmrr.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/ghsbclhkf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gujflwvvh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gmcxjfjwd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/grnrczioh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/geaweokwr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/ggcutycde.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/goqxzrxua.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gtyloovww.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gmnfhmkgs.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gvcpctkah.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gknniptac.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gfxsnlixl.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gclzpxfss.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gtaqqotuo.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/glmoojqmm.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gkajpmlvl.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gehegthuo.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gxkpzyjuu.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/glhadcrrk.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gacdwholi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gogkiwxhg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gxumruykh.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/grxrpeblz.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gxnqpsrin.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/giisoaymr.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gdhkkckhq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gattxquyk.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gvxmgdfrk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gjsylkfpf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gxzdybrpp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/grazpzxfp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gvlxbggoq.sHtML


<!-- 参考信息 -->