代发 wailian999

[D15] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrippljx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gitrubrbe.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyujgotg.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnzpnnvt.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzgayupm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fanxiaobao.xyz/Article/details/gasrojpnw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fanxiaobao.xyz/Article/details/gayubprlq.sHtML

Ruby: arr.uniq
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjngddtta.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvqzwudb.sHtML

[D16] 求和与平均值
来源：http://wap.fanxiaobao.xyz/Article/details/guhsicgis.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gjnswykuz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/groxryesb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gbwdbjhip.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwhkpilp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fanxiaobao.xyz/Article/details/gkpqvbisy.sHtML

Go:   // 手写循环累加
来源：http://m.share.fanxiaobao.xyz/Article/details/gckkfbhdb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fanxiaobao.xyz/Article/details/gmukluugu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxemttfr.sHtML

[D17] 最大值与最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gcaxjfxwx.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gjjbablmo.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/ggdbrnvsp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/giilerxjw.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/godfvxodj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnhjqlot.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/galrwjott.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fanxiaobao.xyz/Article/details/gsrbcyaxt.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fanxiaobao.xyz/Article/details/galtaadvm.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gadgfbaai.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhngirfx.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvlgvcfo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fanxiaobao.xyz/Article/details/ggalesmzg.sHtML

TS:   nested.flat();
来源：http://mobile.fanxiaobao.xyz/Article/details/gsliaikqq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gramchemn.sHtML

Go:   // 手写双层循环
来源：http://blog.fanxiaobao.xyz/Article/details/gozpqgdbz.sHtML

Ruby: nested.flatten
来源：http://blog.fanxiaobao.xyz/Article/details/grijzyfca.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gsoaxkdrd.sHtML

[D19] 按字段分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmchhldph.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznqrayuk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfnhkftc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmcekzdh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtfaygdb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxesnnjj.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxtobfgv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhzeziar.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqnfpihw.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fanxiaobao.xyz/Article/details/gnziriodb.sHtML

Py:   Counter(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gqxsonhpo.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkeemjgg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fanxiaobao.xyz/Article/details/ggfkoxtuw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/ggmuyswdv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjktraolc.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiaeeouc.sHtML

Ruby: arr.tally
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyrlxznz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajeqfscc.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxdabwil.sHtML

Py:   x in arr
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdxyafcs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbexpaun.sHtML

JS:   arr.includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gshcxnwit.sHtML

TS:   arr.includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaglerbts.sHtML

Java: list.contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gwhyanplx.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/ggsuusenj.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaibcldrl.sHtML

C#:   list.Contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaqtnvth.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiecgzkx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gjhsrypzn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjhtwoao.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gchvheods.sHtML

TS:   [...arr];
来源：http://www.share.fanxiaobao.xyz/Article/details/gplgucuff.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaejatmbc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gowddsqfw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjbzcgii.sHtML

C#:   new List<int>(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gjpdagozp.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywsznbxk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gdcdmvybh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gxqdwpwux.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoasager.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkackrnau.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljixuqwd.sHtML

Go:   // 手写循环
来源：http://wap.fanxiaobao.xyz/Article/details/gkyidfved.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fanxiaobao.xyz/Article/details/gngatxzex.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsytkxpso.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fanxiaobao.xyz/Article/details/gddtmuadw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpvfxejb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gpeknudrb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkpmcqhma.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/glqvumgjr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfqbzzzu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggklvvvfw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwivphqv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxwrwmsw.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfssnqcu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbctztgae.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmntporb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gxbtojtdr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhaexgeb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fanxiaobao.xyz/Article/details/grftgomfb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fanxiaobao.xyz/Article/details/geteswfdz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fanxiaobao.xyz/Article/details/glehhcxke.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnbbqlmc.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxhburyb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfaecnle.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gntoepdwt.sHtML

JS:   arr.join(", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gkxdskaqf.sHtML

TS:   arr.join(", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfbzeqmi.sHtML

Java: String.join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/gsjcesnzk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fanxiaobao.xyz/Article/details/gktyfdrtg.sHtML

Ruby: arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/gmwvxlizd.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusfccjht.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhcfmlhe.sHtML

E. 字符串处理
来源：http://wap.fanxiaobao.xyz/Article/details/geozynlhq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gytdnxlfn.sHtML

[E01] 拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gyvulaqil.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fanxiaobao.xyz/Article/details/gxdtagigp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwjlgpkc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtepihksq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fanxiaobao.xyz/Article/details/ggvxgbydm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmylfvdku.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeroyxcf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fanxiaobao.xyz/Article/details/gzzfpzifh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/glovfognj.sHtML

[E02] 重复字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqnbxgzb.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpdzkijk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gocucbdnm.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcnvzkve.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gntlkgzef.sHtML

Java: "ab".repeat(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gejxsgazx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwkjjuby.sHtML

Ruby: "ab" * 3
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjaonivw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfrkjtng.sHtML

[E03] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gcctbivvv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fanxiaobao.xyz/Article/details/guutmtpib.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gugmvyltq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvfdoyxq.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gukgtgpuc.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/giourbtze.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/gdaulxkxr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhayncjm.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gzmqvfnoh.sHtML

[E04] 查找子串位置
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzpypchi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/godtprpwt.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfdamzzx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbewhbsg.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxknncojl.sHtML

Java: s.indexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmoadshz.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmypzoxht.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyveslfq.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuldkhrl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fanxiaobao.xyz/Article/details/gwgobvzmm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhxqrgmk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fanxiaobao.xyz/Article/details/gfzqqqsix.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfldzhlvq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdeolngs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gitwkgmjr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fanxiaobao.xyz/Article/details/gksrnckqp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gmfpdawol.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwboqfch.sHtML

[E06] 替换子串
来源：http://baike.fanxiaobao.xyz/Article/details/gdlluwvln.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggznoggmj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzamfhdw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gbwdiefio.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gmzchsslw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/ggjshhmxk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwttrtses.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbntorche.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/grsytxlqa.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghinfaumu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdniprvrw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgwekqnu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeyfjcbn.sHtML

TS:   s.split(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gshkshkrm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fanxiaobao.xyz/Article/details/glbsedxsg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gxhitlfjw.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fanxiaobao.xyz/Article/details/gevisypfr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaxmcqpw.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fanxiaobao.xyz/Article/details/gmjkhcvqq.sHtML

Py:   ",".join(items)
来源：http://wap.fanxiaobao.xyz/Article/details/gikwmwxdg.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqbsndrx.sHtML

JS:   items.join(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtvcexjq.sHtML

TS:   items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/gqqiizdcy.sHtML

Java: String.join(",", items)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplvejeyv.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqboawmqf.sHtML

Ruby: items.join(",")
来源：http://3g.fanxiaobao.xyz/Article/details/gfdtwlruz.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fanxiaobao.xyz/Article/details/grgvzsxxm.sHtML

[E09] 去除所有空白字符
来源：http://wap.fanxiaobao.xyz/Article/details/gepexodbn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcypswvo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gunxdjhlh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gknermgea.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gkyelmoow.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gynhahnlw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fanxiaobao.xyz/Article/details/ggutucreo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gfjnoyiie.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqixkwui.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiphwguj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gusqsnqvt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fanxiaobao.xyz/Article/details/grpurezoo.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goadaawax.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gwmkmqauw.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzpktina.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fanxiaobao.xyz/Article/details/gjwfvidqi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gotsdztfn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fanxiaobao.xyz/Article/details/gjgpxnxda.sHtML

[E11] 反转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gelnolxti.sHtML

Py:   s[::-1]
来源：http://blog.fanxiaobao.xyz/Article/details/gibgtxtsd.sHtML

PHP:  strrev($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwenmftig.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gydiealis.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gebzywalz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fanxiaobao.xyz/Article/details/glohtbdyk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fanxiaobao.xyz/Article/details/godabmxyf.sHtML

Ruby: s.reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgudxqoq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzgfbtfz.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvwzpnfc.sHtML

Py:   s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqjkwvhc.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fanxiaobao.xyz/Article/details/grwwmrirp.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fanxiaobao.xyz/Article/details/gquongmnj.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqrinfbt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmclfsdax.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdqbsmem.sHtML

Ruby: s.count("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gzjtbkcum.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giywktyms.sHtML

[E13] 逐字符遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/glrqywcfy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlredent.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsahxldph.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fanxiaobao.xyz/Article/details/gsooyupct.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzybktmy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudbyoeta.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gyowvqrlk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpykoxfkb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gthjqiwoo.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fanxiaobao.xyz/Article/details/ginqfdebx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fanxiaobao.xyz/Article/details/gqkxqtmxe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gywnwdpec.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fanxiaobao.xyz/Article/details/gptrlyogq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuzycbue.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fanxiaobao.xyz/Article/details/gfzmwherr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geazboubk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fanxiaobao.xyz/Article/details/gmchstdez.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fanxiaobao.xyz/Article/details/gbvguypfd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhkulygz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gadddubra.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/glydqqqkc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fanxiaobao.xyz/Article/details/glvoifvgm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gxmajwwco.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fanxiaobao.xyz/Article/details/gljlchlch.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gabbipuka.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrfsjebi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gntxvtfda.sHtML

[E16] 数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gsemcvwry.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjezdjfi.sHtML

PHP:  number_format(1234567);
来源：http://3g.fanxiaobao.xyz/Article/details/gjyfodgyz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fanxiaobao.xyz/Article/details/gwycicgzp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpimvhok.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gfgtoqukg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fanxiaobao.xyz/Article/details/gmzrpwrlu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmminojc.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fanxiaobao.xyz/Article/details/grlzduahj.sHtML

[E17] 首字母大写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowbgtpus.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fanxiaobao.xyz/Article/details/gxayvuhiw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gnyxqugkw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkjnbiek.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gxqcilsoo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqbjsxac.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemosmasa.sHtML

Ruby: s.capitalize
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnnsskmz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fanxiaobao.xyz/Article/details/ggqmoadwt.sHtML

[E18] 模板占位符替换
来源：http://baike.fanxiaobao.xyz/Article/details/gufcuyxbk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fanxiaobao.xyz/Article/details/gikuhznur.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhjizhkx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gaaeqmice.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gadyibssg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvthsscje.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouhigmex.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxjnthmp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrugkpwt.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/gytuxspdq.sHtML

Py:   s.splitlines()
来源：http://blog.fanxiaobao.xyz/Article/details/gcneemico.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiodsxjl.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gillkjnfr.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fanxiaobao.xyz/Article/details/gosybsxlk.sHtML

Java: s.lines().toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjoznyvy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gslhjhyod.sHtML

Ruby: s.lines
来源：http://baike.fanxiaobao.xyz/Article/details/gauhgtcpr.sHtML

C#:   s.Split('\n')
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgmjzlyq.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlrdusxg.sHtML

Py:   if not s:
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnhuikoc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxaoehvd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxffmuqd.sHtML

TS:   if (s === "") {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwcuvicb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfpuifpb.sHtML

Go:   if s == "" {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstzeipgy.sHtML

Ruby: if s.empty?
来源：http://3g.fanxiaobao.xyz/Article/details/grolglfhd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/glvjxmfyi.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fanxiaobao.xyz/Article/details/gycbamdyb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzceazxw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/grkyiwbkv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gudfvkvlh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/ggudsohcj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkratnlyj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fanxiaobao.xyz/Article/details/gglzfugrc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gpymdehkn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/grrgzljzy.sHtML


<!-- 参考信息 -->