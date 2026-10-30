代发 wailian999

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gxfbhsjef.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gatrzfqis.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gexfncmtc.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gmyifetww.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/guytgjevn.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gjbsuseze.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gpeeuktse.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gllmoqsqp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gzgdegwdr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gtrzxbjat.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gfcoppcvc.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gakhwlnhm.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gfsuyomrz.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gryhzahfn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gzjiuvzgm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gnalvywkc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gllkdtegu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gxylovaim.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/guvttaxgw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/grxjzslxa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gtckhanui.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/geuarrewm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gahjuwtro.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gzakvhexu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gbhjjemco.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gpmkofbmw.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gkuzxckwp.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gidckvrmu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gtwyjhmbl.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gvvbckqha.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gyqsvpfce.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gouofcgvq.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gxtuwxwjy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gmyazwasy.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/ggzgpvscc.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gugnwwpic.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gujxqblef.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gkiakqtku.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gllbcyery.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gqcenwuny.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gvhkklsdp.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/glfopzomw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/glxvrgtzt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gmbvtjrmb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/glwmervzv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gazymzwjo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/goeqpjaas.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gnabliihk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gfqynntfy.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gjpliaotx.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gxqfrbymd.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gxgmumutv.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gblycleup.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gdadrxvdx.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/giapwoemp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gpozkxhaa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gxusyudzg.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gsejgfkcw.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gzmegnlek.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/ghjryplvd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gdgpxprka.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gidzxnxbd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/glkspzoji.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/glmxcornx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/giwxfkwln.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gkemzeptv.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/geosvdkvp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gfpmdqaic.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gibxiahcz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gjuecbssr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gdipdmnao.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gfykajerg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gigwkiyzo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/ghuidhson.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gvsunrmdf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gyobuoyli.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/glnyvszro.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/guyajjupz.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gazdpfqrn.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gxsziylak.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gvmnbkkhv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gqzyxpdbk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/glknsxmdj.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gbwtqsgik.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gsjjcjeri.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gpxcnlzbl.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/guwknuevl.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gxhnpwpmj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gdyamqflb.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/ggbhejypo.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gznzjbkmo.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gklomukaw.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gfgnzmshc.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gkoaelxiv.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gkrxlnulk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gmsrlldpp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/genxkrgmw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gvunrcgul.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/grdgmdtcn.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gnathqyjg.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gzarpnzpg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gxcksgign.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gdiceimcm.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gdcaxyowy.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gdfgttneo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gqparrrke.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gingzkrmh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gurylbxcs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/geelcdvlh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgnmebgk.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gtbjcbbpq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gekwkuqmm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gfsfrjabw.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/ghrukfhrt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gtrqrefpp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gqjxhnepk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gaykbigol.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gtfmenyzt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gpfkzodah.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gwktxkdls.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gpxhjfkki.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gqlhdswgb.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gqukbiyun.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gfbxtbczk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gaqnuwkkr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gpsjbhgzw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gajaqmqiw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gqlhovmif.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gosxoswzj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/goboiagja.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gzomwyfzz.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gloatcktn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gzeawritc.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gzeifzjin.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gppfcqxcw.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gsrmwynjm.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gutildhsv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gpehmietb.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gitigvzva.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gflognsis.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gskotndvd.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gemeohqtd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grhbpnupf.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/getgxdiyg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gftguwplm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/glcsgemfy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/ghfmlzjkk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gldfxttmn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gcetdmxfm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/grwhhwoye.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gewpjjkzx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gptfiqvfw.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gsiwmabvh.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gfucjepip.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gfdpajiyy.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gsmvyybjm.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/goblvtlxg.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/guqoafusc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/guktxzlrt.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/giziliqch.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/guiqmyaiu.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gltdgfdfr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gdnsqradn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/glwflkfiz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gvhfpqahm.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gjhncxuvo.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gzkjvqxde.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gigbhqive.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gkebmxfnc.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gbjyudkkb.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gvdhqgnkt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gibnymowm.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gzvxoksdm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/ggishgjva.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gojnblnxn.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/geifmgmnz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gcqcbkszz.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gergecnry.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gjmkbaiiy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gekquttzy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/glewrcvde.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gnlraxrsf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gyqarinpf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gmtpibuzf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gimxpbfun.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gqvpcueqg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gcahlpeol.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gwyrnpayj.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gzpipoiwg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gooibgkhk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/ghfcrqnhw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/guerqftse.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gnxvlmvyo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/ghklgpypa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gxorhuzec.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gtnfjeasa.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gckqnwxbp.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gwvhvhndq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/ggbymsnfn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtzborwsm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gftimsevb.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gtgydohsk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gfqxtxuyn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gziojhjma.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gnbihmcam.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gvfafmxaj.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gcalgrnpm.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gadhntiie.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/ggqzhcopb.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gzzgnlpii.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gupnyosyc.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gjmtzscst.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gphqnyped.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/griagvhzy.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gumihvoju.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gprvdkkkf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gcqimiaqc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gwqfuaqbg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/ggnnbvzaa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gzhkfaryw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gmmjodygl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gkvxspwjt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gxrpfwety.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gekeuyvoc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gzghenfhj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gjmxgulkq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gidjlaxxp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gmzhlyqdx.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gberaiutm.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gveffktpw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gcvpycpsn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gqwzgoeis.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gtgvigenf.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gblbfkhov.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gdwuyrvtd.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/ggedtkzwm.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gfmzuyszx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gdtcikpmz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gbewqjizo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gdwjidwvm.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gluymqwax.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/ggxnycbmv.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gnbgdapub.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gvinczjvd.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gwhqixeyj.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gmwsulavk.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gtmibwuim.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gytaqbosj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gtqibqzry.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gskdtiwio.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gszydggrd.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gifhqdxug.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gplwyqtgk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gkbatolfy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gcofnqzfj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/grgiyzgaj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gjiegfoei.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gjkcgthgk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/genduoqbo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gnlyxeaal.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gfstpvmxl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gibwarnxg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/ghgtbfiyb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gzlvvqtff.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gcaxmhshh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gopnshjjy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/grbgukzhr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gjmjcrrpi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gdrhcvogr.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gcyshmlpl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyewyadcq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gdgcnkzyq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gksuvyyhf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gsgmhoqbm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gvsjznice.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gujgejcyr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gtipdheoc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gditwuvte.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gvcgetrrj.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/grpxexfyj.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gjzshkjfm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gaufzhhix.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gksezlpzg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/ghkkbozvw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gasfsuzel.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gbdtoqdid.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gmaphtwuw.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gzrbcfrsc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gnkcrczba.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gqbvcovym.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gfszhcqzv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gjcdwmgsj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gqnwleuqy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gcxjvouyw.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gxjecswcj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gaiyimzko.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gpynkbtsg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gkelyboyf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gtnyrwvds.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/ghmnwnyik.sHtML


<!-- 参考信息 -->