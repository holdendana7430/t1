代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gvaowfjzw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gqhuyuhbp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gkmdfjujb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gpltbapss.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gsxwcqfmf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/grntpjqaj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqhfwtufv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gcajdhohk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gcljthqnk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gmrwyfjwi.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gnehvbltx.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gkfsplzfj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gacyctiov.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gokcgznuw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gavsbofza.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gkddkrlhw.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gvvywirhk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gbgiuhagp.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gnelphhlv.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gfgyrdfez.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/galhnmeqg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gevjlebth.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gfmbokcgu.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gnznxzlff.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/glfkvublz.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gprfcvzdq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gouhmgezu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gqetuokql.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gqbbduawa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gqmgitqyi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gszoicefg.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gjngwqyhf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gdqdzbiri.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gftpqyxbt.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/giohtztke.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzdeykaua.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gjhtlltpq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gspexshnl.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gwsqxjjwb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/glajoaopk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggnnpklyb.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gsznvyrow.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gfoqghyyy.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gaftjgrpt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gjebfbpte.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gragteabx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gutkgdvzx.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/guiycpwaj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gactfwpfo.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gqkthtpdy.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gozmmctim.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gmfevftly.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gvjkdrafa.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gqsqhusji.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gufhjyuhy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/glxvxvybs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/ghbjmlujh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gqrjfkvvt.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gydkqozgs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gitalgpok.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gxzeitxkr.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gyaodqbhi.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gaunzhmnt.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmbkkzsaa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gxrfsrrul.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gvwyhsyvz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gsprzprgv.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gniumbxdi.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gbtbostfa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gplvxqtvi.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/ggxqqzraw.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/geubugrit.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gehbptucl.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gvuhhxlfx.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gwdwurjea.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/ggutzbsyb.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gpuxilcag.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/grphhqyba.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gmhxgyriu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gedvdgqkx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/glsxwqmax.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gkrgndyjx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/giebnmhxd.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gsvljxrxm.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gssxfpotf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gcmkebnpx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/ghlhdpsvj.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gaogldpzr.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gcuwnmcjz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gkcchbeab.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gtrjsumqi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/grikhpghy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gtsqczjlc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gjhsieacc.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gffceqaix.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/ggjoyzzcm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/galmogvdi.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gvgyftsgw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gmqaqimtg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gdsbnxrzt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gbqoshpvs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gdetdzadm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gcbccenpm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gmzkphwby.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gaoyezhcm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gkhqjyzyc.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gszrbclnz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gygqtnopd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gyaxheblx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gvmtrijdj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gynurzmhw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gapzcxdyt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/grctvrobx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gglgxcyky.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gbxxhciys.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gbffthljy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/galhpjkhh.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/glalgjqbw.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gvxccdyug.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/grqemrzwr.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gcwkqqrgy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gjnrbrmke.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gatxsnbdd.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/ghfgahhmr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbkneqnfv.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gqfbmbtmo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbfnhtosj.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggcmpfvjj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gujgdjdal.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gpbxfsbjk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gqxhobeud.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gcolmwuaj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gphgsvxid.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/ghrekkuxr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gqthkfkdh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gdmzfneae.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gvdejdiaq.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gackhhzjp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gycsyqcqr.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gqmlcawig.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gqywtrbay.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gpgubezbe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gjpshiulu.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gqynpaevc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gblokxwrs.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gzcjruvam.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gywcwpfjy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gkqwxdlsk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gccuzvhkr.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gjaxcmork.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/groaodxps.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gixmcugxs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/goaoqcmws.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/griewkhlh.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gplfvdzgv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gjlicwfgm.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/golxxhkbv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gqersdudc.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gqeiyrojp.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/glznuuigh.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gtgigvmpc.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/ghwooxtce.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gebkxlgke.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gpehownuk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gzfwhpwow.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gixyjrfeb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gzdgumjix.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gahdwjlvv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gvgjvrlzd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/goasgjokk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gdhnhehfe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gzucgkjdd.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gpimfjcpc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gjohrlrko.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gbmkxfmxd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbactlchu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gwrztgdtl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gkqdunxxg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gxxhyveah.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/geberxopj.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gempwszwb.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/geizqcogz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gztfnerbv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gujtnnbni.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gelwzkyry.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gxvimgcrp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gsmnoazta.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gozmjqwaa.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gkfoqxxjv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/giskgtlne.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gheaqebmk.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gziyeqsfn.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gscnrehtw.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gyldxoutv.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/ghlpdxoir.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gunmraddj.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gxdbyviqs.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/govvqkfzy.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gucacszwf.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/ghzmjhuth.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gdutqwtde.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gmcpnqvez.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/grmydioxq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gmvzxnufk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gtzygppka.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gumgwltmu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gqfqjbztp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gzzqhpxgt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gutrjgkpf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/goyisqyid.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gbdfkrkok.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gsvdfirsc.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gpqgjyxvz.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gellxjibn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gqdcgqemh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gijjhfqjc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gewrfaboj.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gjmehwcff.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/glmqqgcyx.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/ggyusuens.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gvywqogge.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gnmvqcyim.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gztyfknld.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gjnqnfhbi.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/ghiycjntb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gvlmtwbzn.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gmwjlaebx.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gznccniio.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gciascbyk.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/grcsgstfs.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gfpfhscbr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/guamiocmd.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gxhawriom.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gevkcmepn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gsrchjkbu.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gviwojerv.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gchnwepsy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gbjygghdv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/geaicvsmd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gazdldvop.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gcotytzhd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/ghjlflncb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gyjisxdfk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gcquakbcn.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gwwukgdoc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gnmmhtcup.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gcjbhxmba.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gasnmgehh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gewffglmn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gphfoqxoq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gjkoyktmt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gbynfjnkc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gjwwicdxb.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gklzohepr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gdlqskgce.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/garrrpokn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gkasjluok.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gkgggyqvk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gqlddjdfe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gkpazzcii.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gmyhwmoyk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gsrezbqxv.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gqkphszqa.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gtnsrvdgk.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gkrblxwrs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gjrzxvyoa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gzvxqyenz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/guybajpah.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gwbebydlg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gemspzuwo.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gybjipzdu.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gwcjxwufl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gixsgnqbq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gpiaqqibu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gmlouaude.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxtcbaxit.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gcnxmmqid.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gocoqodyx.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/ghlcqzzzw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/glehbdehn.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gcdtzkrzx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gxwemsszk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/ghvkptiph.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/glfikrwfm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gwgnwcngi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gppseohgv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gvuquixrc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gsoesxbwb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gizngdpgo.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gnemmezbp.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gnaabtkln.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gbkkfyjze.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gdgzahrua.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gbbosodvo.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gfzhfdyck.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gfzfwxnhv.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/geanvvilm.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/ggfkhbrvq.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gvvbqdhce.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gunltfkvl.sHtML


<!-- 参考信息 -->