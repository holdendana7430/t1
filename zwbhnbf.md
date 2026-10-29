代发 wailian999

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gfzjjdzhc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gmlmwumnn.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gdfozqqgg.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/glqbjvzvl.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gpvolwsxx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gvnrswgdm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gxxmaekha.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/ghmeewqcl.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gipmshdjd.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gmvfmyfhc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gtnjmzzdj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gvedleczo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gwkmqccwu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gosrcbeyw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gswlyoblk.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gvlpphbkd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gudgqrwrw.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gzfpqdbsr.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gmffmnvif.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/guusggtdf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gddxymsxh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gumlmjbem.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gmgxgaltm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gmhyfuemm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/glayfnlwz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gkuyoxgrp.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gqhvkelos.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gxlxytyqn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/ggnnyriwd.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gonjjfksc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gztafgelm.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/giwpizmmh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gmhwelfmi.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/grfkplkew.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gbqashxoj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gujrnysue.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gtbztntfj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gfycforlc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/grqouujao.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gplwjynot.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gkmxizest.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gzwojqsbc.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gykkurusc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/ggcorkdco.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gxnhypshf.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gczpiplze.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gcrthiqpj.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gjfeocheg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gzwvzqpwr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gaqngugwy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gvzaxhgrz.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gjpxposvi.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gsthueyag.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gsulckdks.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gfktbqwtl.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gvdbppryf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gyqkfliub.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/grgtwpwkt.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/ggufolnzh.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gvmgdgdol.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gtmihjtzs.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdpmlsjpc.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gqeinoatu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gtkahefww.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gkegzkpwr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gblqanlmt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdqbzmghy.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/glqdlyhxx.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gbktxdmzq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/goxohudhd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gwkvxvfgy.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gthhlxorf.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gucxigzbg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gpequlzrv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/grxygnyye.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gmlrsgtva.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gkieduxel.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gcthfjdyf.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gvkungxif.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gyssmyuos.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gljpspuhk.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gadjdhiui.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gmmoijvye.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gtrmfnezn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gedsrviko.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gviayhgwv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/ggitetktf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gropkldzk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gardcsned.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gaquhwrgx.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gmrybbift.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gtmufvtmn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gozhfevec.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/goswzrltt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gzjqfspjn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gexmevrfz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gyqlfrspe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/glzdacxzf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gzqvhxgik.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnarvqcie.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/ghjpkvihp.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gyyifyyrj.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/ggcpfxxcq.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gbsfljlsq.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gxmdijdrx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gfziwseom.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gwnpimdwq.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gqmmbewxk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsltpxlnk.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/ghwjxiylp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glkomhsmv.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gsgolrblv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gcifropvt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/glynynjuv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gslhgnpie.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gwfkljtns.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gtvxmggek.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gypfadrgb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gognuqmlq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/glcvfwqsi.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gsvhbitun.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gbnfaolsu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gwzecjfsh.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/grbqlzhkc.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gulcqicgs.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gxvdgjctf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/guwppypkh.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/geqwzilio.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gklgbqkct.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/glujfjpdn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gugcyryhz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gzhinxsqr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gcxkzkugt.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/godqnbcwp.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gwdovhmqe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gyouiojvn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gieoodhtn.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gjapebgai.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gfprzwclc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gydkhqftq.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gkbxjbgfp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/goyjywqzt.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gbbsupvws.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gjscsnhyc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gpubhhldt.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gfdwesyvp.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gedgqdsdc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/ghxmvuher.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gjuouakvp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gqimjfbzc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gzluyamib.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/geialtjul.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/guhitgrqo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gaxcnkadz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/ghegccdip.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gcauimmvj.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gacpagxic.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gajzxirxr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gvhydnquq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gkqlupinp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gerzicfte.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gbhwnoelw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/ghaqmtghw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gbzrpvxyp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gcfjzoyhm.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gxvqowemi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gzifdhwgs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gjeulglbt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gunxagwsz.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gutrrvjcj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/guscabtfp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gogxanaua.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gysztwbtv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gdyznfxgk.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gsuodowwr.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gbhhtzoia.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gdhuclpaq.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/ggqbvcigk.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gykzkhwka.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gnudarnzz.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/glkqxtejz.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gksfsvgma.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gdkknrlhk.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gviboxpwt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gxviliagm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gwmzsmzzu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/ggfpwegzv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gghpwcbqv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/grqordsgz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gagfieacl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gyczicvbh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/giabtpnsq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gfrcomxac.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gioluxjof.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gzektmlfs.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gyfkronyd.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gstowkevw.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gjlwagckk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gmsdobkac.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gtdryydym.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gyqysdxao.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gyukkziki.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/grtxenafw.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/ggrvruuyh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gnoghubdu.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gxjcwhjfy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gauuwowrx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gvpktkase.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gebjehqqj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gnlbnyhrd.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gnnujamef.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gxrvacwur.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gkuolutwe.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gnrlxczkw.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gviiwdhpq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gscwxhviv.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gqdpzwuif.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/ggyjzozre.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/glduxxxgz.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gdnqcwsjn.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/geoihmwbf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwsoephkh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gmjlhysbf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gkpidcnqc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gigfrzdyl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gvkkhxwwa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gxpptutmd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gouemqnql.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gpnsrssug.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gjwmyguqv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gchgzxwdl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gzqorketi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gnuuzuuoo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/grfyvorms.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/giowkslom.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gcssyrsdb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gctuneayc.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/grurivury.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/grqzymjpj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/ghlnojdyz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gtqhnkpqr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gmpunbutf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/grgicxcyd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gmdmoutei.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gupuxqbjf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gvlxlmdqe.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gatgyrbbw.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gzxdvqnje.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/ggtzfxerd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gbnpxwmrv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gvzegyscl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/ghinzfiks.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/grfqvosim.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gznenssvl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gzqdjfniu.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gdjcnzjaq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gmpznsomv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gijqomgvh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gwkuxwaaz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/glvupcoof.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/guneldzup.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gzcwueioj.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gnqqrgyhk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gwsgzdgfe.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gankwayqq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/ggocnbzde.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gflnqwejv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gjoupxncn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gdhwzgqgh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gcumedhgn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ghaifjrcb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/grhcjgmzx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gdhabargt.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gmbupiqkk.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gyjixgfss.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/ghwwmjmut.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/grrptnsav.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/galiazekg.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gzpjeqyxw.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gxfblbdbq.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gytoemmyr.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gspvqglfi.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gvrfqjytk.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/ghwkjkzcv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gpqnmarhm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvrerqygp.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/ginhqqtvx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gagsssekv.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gpqddcayp.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gxfzqfdtf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gzjthdlas.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/guchonubc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gapddpufs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gtjkqxiyv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gvhteszkh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gkolbrktf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gqlqqcepq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gtsnopnhh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/glzcmhuzj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gvuxzwklh.sHtML


<!-- 参考信息 -->