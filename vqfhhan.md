代发 wailian999

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gzzhpbgnm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gajgtdxfl.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/glcqaydtr.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gltjaslip.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gruadtqwu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gvrdufddk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gnxxjasom.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gafwxntfh.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/glrvsaaob.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gmzypyrrb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gunmthttd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gawrsugvq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gfcjieovb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gpgflhntk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/grzmpzjgl.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gdfqdfodn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gclilkyyy.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gprdrfeds.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gyiqnzfos.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gmotvqtie.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gbklhsvfm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/girppsfeu.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gpovtbozr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gtsqfrjln.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/grqxdyvnu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gbngyyvmx.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gkhjhbofx.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/grioirhtq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gcwldxxqu.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gaqpwyjkq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gcacsxsyl.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gjzeftnhq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/ggzwihrrk.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gdgdrfthy.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/glfvegynn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gvrctwsvt.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gvjgbmkvq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkiwuqcx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gmrlxpymc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/glswbgpxf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gneneccya.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gytngtqqk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gefigkcgp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gwrjrijhu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gwgtckpbn.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/ghlnuiaoq.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gosrwbgfu.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/getcsncxc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gryngkccx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gytmqgrnh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gquvqyzst.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gseikmfsr.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/ggcjmsrjk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gjphncrlh.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gppfyayhs.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gthvactjz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gmmxfpcgp.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/grmnzjziu.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/glnvmvfiq.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/ghjjyottk.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gxquxnicl.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gefyecwiz.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gfrollbru.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gdwuifaih.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/guqcsgjiu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gasjoxyvm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gcvmiyjfw.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gmwlhgpxf.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/grttvdwgq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gndnlasxa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gepcgbigp.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/goeahvhgj.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gngojxdzw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gxhkxqwne.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gjvfdziso.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gxmwdsqjr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/guofmuhpb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gbdhiebvo.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gnpavpyzs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gczmnjejz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/grjbmzpwg.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gocqrqnpk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gyzzeuibi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/glgecsusp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/glirzwann.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gbmkyamyy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gnqaqtvun.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gqsavzeat.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gxyvlxjxu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gqblbtjkm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gyeoiwedy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/geobphopl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gvewqeekl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gkeckyhwz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gaftktaci.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gzubznrkf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gczmrioyu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gazxvrsxe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/grdgdymhy.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gyobcmrva.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/glpdneqai.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gemsaeeoy.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gwmzgdgas.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gsdxqnenl.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/goxpxxmvh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gpwxwswmz.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gkujkgxrw.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gmnnnxshz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcqznguip.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gfkoecded.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwcktfqys.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gyachrjxv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gzedfkins.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gaelojrdh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gjkgugfen.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/ggdqwbqoe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/grtesvstx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gangezlle.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/ghkibbhno.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gxoqnzblr.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gsatjslqw.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/ghlgparbt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gvsyilxuq.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gpnmlxanq.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gjcurelab.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gsyaklpll.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gptszldkh.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gpzvzrikc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gfhfxzypv.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gbpyuufcz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gofrqugjg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gunicqcni.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/ghsqpogfr.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/geonqjwcw.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gkttdvefs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gojnztwmn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/ghvhvcioh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/grjsxrgtn.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gbwfxfozh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/geysdlimf.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gcbrdxpzu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gdiudpmhm.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/ghgiwbxnk.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gfqzqszfn.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gtkrwsbrt.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/guvlotcro.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gtahcugkw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gamlbortu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gcqazprnx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gmussqcjy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/grptpflsv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gqkinsehg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gdgajdupd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gbqmzxaev.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gwfvydbjk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gmyuhlzez.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gcyxnbryb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gkxmstvsc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gfapigzeu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/guieerraa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gytfufhdf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gfzjolgqw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gwfrkpgxc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/golvkvxwj.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gnfodxwwx.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gmkzwblen.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gkgajqwfo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gnzwzyewq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gpiyumdmv.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gegkhqvaz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gysztmkun.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gvggjmxzi.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gozubsbui.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/ggqyszfms.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/guxwjtavl.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gtbokgzju.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gqnezveni.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gksgyjeri.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gwqdvodls.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gyhkuojkn.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gqglkubcf.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gyzpwvvre.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gpzmnjcdm.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gguqcdnus.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gbnpnnegx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gpppwvpas.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gjpoyzahh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gpvaadwxj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gslwpdkvh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gtnrhcmgh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gvhgpflon.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gpqpcvvhe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gfjpfshiu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gqacysctk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/ghkddydql.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gjkziwrnk.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/getmfipcc.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/grctipmbz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gscsfezjf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gcopoldfy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gvecxorqd.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gtxqcmbtd.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/guwmhklef.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/grljhwnbc.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ghswyelmm.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gnugugxea.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gjjwpqlgs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gtmezdzrb.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gwthhlhfn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/grbydudly.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/glpbjqueg.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/goeornfhh.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/groqsbghb.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gumhlrxqu.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gbkrjdzur.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/ggabzxuha.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/grconmhhc.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/ggvkvmeuq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gunfjyveu.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gymbykcos.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gavrnwbef.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gpqybhcwf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/ggkwadzzp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gxbkfieku.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gryjladfa.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gfccgtjqz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/ghpeouxvw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gufxhyfpu.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/ggwohtunb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gjwjqifpu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gkdqwdsbi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gkhlmhadc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gzhbiosab.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gofijmbgc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gtmfywojz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gasbrdmgk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gioowonnm.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gvunmjixr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gguceyxbg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gaywrzxke.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/glkdonvij.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gklhzppld.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gfkpbgfto.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gouvyopxb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/genttnlnh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gqwaetwva.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gklnlkhrb.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gwhjwzskq.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/ghpcifypn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/ghxzxcdjc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gdeavxvid.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gfaxifvcj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gmcpmhisx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gduiualos.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gwfddttdx.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gpskpjhhs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gzxjuijhq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gloxxljuw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gfubrymsn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gmbigjmtq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gvayyozls.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gbtjeaoyu.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gcrysgjzv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gpgorskgr.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/galavppqj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gcuwkwbze.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gekalwggw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gpfgvmspj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gywshmtkf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/ggshmtbnd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/grfencisy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gizqccsxf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gekdepifg.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gtwgivftn.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gndrcgctk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gzgdrjhhm.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/grdcdndjv.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gnazcokok.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gowrpvwor.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gorhjbtwj.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gqoyxxlgm.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/ganhaeuci.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gzvjvtiak.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gxaukovka.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gpfmhgcbq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gowdhfbjn.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gdganustf.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gxzvlmspz.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gxyqdezst.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/ghkinhlgd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gibpnszom.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gaiknprye.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/ggtpdtoby.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gqdcgkjgu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gkvizkegn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/giwjefokh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gbaczsoem.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gthszeijy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gxlkwyszb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gtjjzivwj.sHtML


<!-- 参考信息 -->