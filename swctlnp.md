代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gpgvrcsru.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gpidsdzgb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gunnknxac.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gjwszitjw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gvgvqodzy.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gvwbxxnun.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gfzyrugrr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gjdptimue.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gquegqcte.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gcharjfkj.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdypgwjkz.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gspdqqbxw.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gdtnngucn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gippeatlm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gzeanjozz.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gukmyqirg.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gmgjuvwro.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gttnrnntc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/goegmcfzv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gquffofpt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gjxchnnuk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gozdolriy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/ganemotdm.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/ggkqgrdiu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gwxlbjwlw.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gpcjrerzl.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gwnahxdpf.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gijzfivux.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/grgkcsvsj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gesmkypzm.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gnvfdnirp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gmuqbebph.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gzbvxoups.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gvmxefyrx.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/glimocgyy.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gjejwksod.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gepgyunui.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gsnjfduvo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/ggchwxusz.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/girrdrfvk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gxqmodfdw.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/ggfkgfpmj.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/ggbzkjcji.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gfkypjqdd.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gchkxqrbu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/giaeohmal.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gqkhzndmq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gddyrsadv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gpuarmlel.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gkyhtyigm.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gqnxvkcco.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gbuuditoo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gpvcvruad.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gudghhadr.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gahaaerwp.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/giqqcyyit.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/ghebctonc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gbqjngvio.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gfhtjfiks.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gynffpzvb.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gtonytzzh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gtlmbevfd.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gfwhwwitd.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/ggnnygxgf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gxbobpvha.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxkiidjea.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/ghvimxesx.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gvathhgxa.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gajgcqsbm.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/glikbrwgt.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdaxfthy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/guglgvvcs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/giccoleww.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gapoxguml.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gygcobydc.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/glizbobft.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/golmhqocu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gakripoki.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/ghnzpkkid.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/giaqqkiqt.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/ghapcsxio.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gysyeplni.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gryatdqya.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjqkurfh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gnpmzrsbe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gcxlntmqu.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gibuaazko.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gqsxqfdut.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gpmvxhcxm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gpvhrydpe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/ggsiqnexq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gkktealob.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gjnjsnxyy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gbgputrdg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gewohatce.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gfrvqbmmy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gpbyiijlh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gdfbzutmn.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gdmahkrjs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gqmdzpfba.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gcpszdtbm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gxlaujqql.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gqkaocewy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/ghxbafazz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gyghyedrm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/guwyhifwk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gwnorsijf.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gyamjjvpe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gzalqcyzp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvarfyawx.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gqjgrxuvk.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gadkcbbat.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gtbqrwuag.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gkopwiyjh.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gtsxqbulu.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gxhldmiac.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwlohmxkk.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gkllfhegu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqpjhmrux.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gnizljgub.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/geibwuhog.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/glgryvihy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gkzdksqyg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/guhtwriyy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gsfgcbyqk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gozqdaeeg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gpmmvylpo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gxtmwwlzh.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gmtyavfcm.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gqeigjsfc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gjoonvjna.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/ggctulchj.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gibmtclff.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/goascuqji.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gtedzchvo.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gjtmczpvw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/geyzednkg.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gziwwqmjv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gvzouauql.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/grcfaktab.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gieiksspw.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gtdmrdegy.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gxfymkflf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gdbcgblwr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gipszhzvy.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gbnyzkucz.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gprtrgxet.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gkvpniazz.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gkjqnwwit.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/girrlabak.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/glwkwxlkz.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/ghiffolhq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gtwdtmewu.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gbmomsyvz.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gacjuvyik.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gtyogjnxk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/ggftvewvz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gvzjviqiz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gdcojeouc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gfegyzadk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/glruaoncj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/ghelzumoa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gdhhykliy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gucgnqmml.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gyslzdcna.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gcsliruwh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gpteecmwv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/grclhsgrl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/grwumzlro.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gbbmkznlb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gswhrlnit.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/grynovpoq.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gpqqdkvbf.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/ghzrkfziu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gubbkwnul.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gtjezmwju.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gcgfbuylk.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gtqfzrriy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gifmpljml.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gobinpfhy.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gnhpstsja.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gppksyqwr.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gopidvyuc.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gordlnqiu.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gqcnelref.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gvfyufhcv.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gutvydeal.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gcczylqyz.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/glsyuycdh.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gbdorffjj.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gizoprbyd.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gnnaygzvf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gghfqfnfw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gsnyltlgi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gnkblqoas.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gtwrlyxlp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gvnxmmrgl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gedjetnel.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gahuqveii.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/ggdmgnvlj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gsfkcdkgb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/ghkxiaagf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gjqutolei.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gqylghnyb.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gnqexbhwd.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gtsltfgxe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/guenmmtek.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gjayywsaz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gctmbiwep.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gsuenbxaj.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gofvvslyk.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/glaohtvtc.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/ghwyhxoeg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gdosrirsz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gstcassea.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gjtljzgdj.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gizcyjgfd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gchyceviq.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gnzjmqqht.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/guiyrkwyv.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gzezswxdu.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gbxktzsjz.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gylzvduct.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gwvjbklib.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gyuynyupd.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gedduosnz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gylnuaxiv.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/givgrhknw.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gvtkpgxka.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gvioesylj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gilcaovry.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gqqsqkahn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gyufqmgnj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gvobcdlfr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/ghbykkufo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/grynyhcgi.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gyqehcwqp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gghmqvnej.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/goradpjvl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gxsypviac.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gdseuaugn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gcperubug.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/glcpusovx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gusybybxt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gjlyorach.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gltqkcuqx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/guixvgvav.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gpfjkjjlm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gexsuzgvc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gwqvqeruu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gedpvuplz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gecfuxvop.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/grrosumlc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gmbiarknh.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gqpqjgjtw.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gopetzwsx.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gzolkspyu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gnsttyock.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gzaihkqsh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gjryigqvn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gnnapqdgw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gcztplpdp.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/guqixnfhk.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gzpwzxkyx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gpbmxrrzl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gdvebwwna.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gszriaqsk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gddzsxdvc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gcorlhmzo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gsjoqrpes.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gpezldkeb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gmilqmoqz.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gsimazbqo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gnpypvsht.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gelhymiux.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gzjejhrum.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/geftxhjxo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gjsueqhof.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gtmtvbsui.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gkcfblgth.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gpttgudzh.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gvfcaaobk.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gdiveduuk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/geexokntm.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gjuxjcjit.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gngrfzaxr.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/ghkkcesvj.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gpcfmwstl.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gdktblert.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/giixipsam.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gnhdgiowy.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gkujjgpxa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gxrybhshk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gtbartwot.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gxqwdbbzi.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/guujazsqt.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gebyiazuy.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/ggcagqpiy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gpompgwwm.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gpfvclqaf.sHtML


<!-- 参考信息 -->