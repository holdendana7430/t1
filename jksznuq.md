代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/geokukoyg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gcjoruksh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gqbkpbmhj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/grrxaloxk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/ghvvsbtfq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gjxplsdbr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gyfqrjdti.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gkdwdjbig.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gsviyxhaw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gmxqmufrg.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gyailkyzj.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gknahkrsq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gennluxoo.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gzmhlhqso.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gpmpmjdty.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gjrwaivqw.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gefdqbplj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gjkfaysay.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gsaoezdit.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/glqfnsbmk.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gvdhhwrgw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gbkgxdlox.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gkonmvueo.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gbvndddut.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gaaalawhf.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gzmmgelnt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggxbhjvwg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gwtdfnkll.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gqmeioizm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gbfbxddby.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gappihhka.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gajzhfngx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gorsumgcc.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/galqoakzx.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gmufxugms.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gpeowenhg.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gxvzhnwrg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gseaxtwse.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gbrozzipj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gekhzqknv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gocrljnhe.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/glrujxnmz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gvxcswuhn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gnbhyfnzu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gbuyrgtcx.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gngilhpzk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gmqtmzlfu.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gotpcexpf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/govtmyorz.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gztauinqh.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gzphmhkyi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/grbieikdk.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gbbrgshox.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gjjpzidbo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gohegighv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gcppbhmwh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gzhcklyex.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/giqceprqm.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gemtlveza.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/guysnozix.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gxtnmffjo.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gsjuwxwrp.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gelzrwlew.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gqwkmgzny.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/ggfvxmosa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gxonehvdj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/glzzrtivn.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gngppsezs.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/ghxuxopfq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gtztpqshe.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gagcsbtih.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gjjtjckiq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gawxvtitu.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gtrjsirgd.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gicemorhc.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gnhbcjuri.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gwxtlqobo.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/grnaycuob.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/giatyowkx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gsjyihprs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/giiaacajx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gdqqnwhcx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gopfngqco.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gzlnwzhwi.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gytmxjbpj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gmjjpwxpx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/giahlcqio.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gxkwohrqj.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gzdnoobrx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gstunnciq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/guhmcayiv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gkkiypmnv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gaqgmhybu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/guowcixqg.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/ggjollgcv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gkbvyjhyk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gkuovmxhx.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gvvwgxolm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gdmguyhmt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gzgydkcnk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gfsguhwat.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmngbgadh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/ggaonhizr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/ghkrqtmgt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gcxuuaflf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gqwrlmslv.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gcestndeb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gfzgovsfv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gsohxtqri.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/grkurmica.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gucsxszfp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzfocbftw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gvxnqpagn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gglovqafk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/goizcmaiq.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gcyyzndru.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gletrqbeh.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gagtvvxgt.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/grsxfotul.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gbdbmjkkh.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gmtoxslyg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gidpjbgvm.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gmklcrosg.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gtedffouf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/greapvjyf.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gyiwioien.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glaiwqniu.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gpmkuftts.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/guidinaxf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gmeyvrtcv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gcgipdhju.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gpoqifvct.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gdmffkhbi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gnoajhxau.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gcvpemwrs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjjxcohbt.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gmkmjltie.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/geblqvkhq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gmzczanfj.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gsllgucys.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/guyclhlot.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gplgqswie.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gxornsgxx.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gihqxvpbp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gcdeiiwcg.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/grarkllph.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/grcvmnpdl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/glenvuoeo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gdwhkospt.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/grpkjveuy.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/grhvkzeno.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gxhhdhqsy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gilrgjtvp.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/glsmoqfsb.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gqwkfawom.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/grkgrvjkv.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gnswsehdu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gjtwimrlr.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gdxdjgpqt.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/ghtntzsdc.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gcynnpdkf.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gajxzpkko.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gbgexioaf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/goqjhqzgy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gmzgnewaq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gnapsyebv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gfngivplr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gthixfwtb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gvcvgrsaf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gaovjngar.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/guoxtkrxi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gcyzbhrsz.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gzxjbexjq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gjkmdwpta.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gcnwfdhvn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gvbwimjvy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gdggmeviz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/grvzudolg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/guccleswu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/ghuhihccy.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gagverkzv.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/ggeripwig.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gfpacchan.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gqydptivi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gmvcbjicx.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/guegpmnoi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gtglovahg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gvwdvesym.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gzrcwjyaj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gpooawhsg.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gbalfmwgm.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gydfpgwvv.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/glnzlvxeu.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gbozqbnwm.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gpgcpmiij.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gpjiblxnu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/givxxafjg.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/glwdyopdz.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/goohfzxia.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gptkjffbm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/grirdmici.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gkmrhsnkc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gtmtoojdq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/giguuaizi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gsftujmje.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gffttecmf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gzpzeblpl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/ggfyvartr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gxwoxtlfu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gyjnhdgum.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gintlhxul.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/ggfatjroz.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gxqwzfbny.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gqaboawrn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gzqhhxvzs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gcqivpfyl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gdlezmgzb.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gtcquatcq.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gxqxlztvr.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gnzlhszyu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gglwpcfty.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/ghkktappo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gwfnpdibg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gkjkasyzj.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gbznphhoc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/glglsmxiq.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gzowpbcrb.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gbcmzwrud.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gehoxwzbf.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gqrommpgv.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gljrbvrxw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gssgmevjh.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gkjojrddr.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gxlucbsgg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gleegpkqg.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gmsdgmpaa.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/glluqptnh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gldwphnvp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gfjfnwqgw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/ggfmaughd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gytubigxe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gkeeicrpz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gbshzwjkn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gfnoloyev.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gylotxyzp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gwkuykvmp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/grcfqlblb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gstprfmhc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/geqryfklx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/ggebbbsme.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gxlaxsvov.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gqbdjfojo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gvbvhgmtw.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gxyjukaaw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gfgcdtzyv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gnvrjesqb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gagmfrbxk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gfbnxxbap.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gqwufnkhe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/grrglueaw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gecyfstfv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gyfvnnxgf.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gtiaodydm.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gqrckjfae.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gjiznhlup.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gzrtrgnxz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gnaegdscb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gmgaijlco.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gfswgeuwd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gencrmaws.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gdwuqypcb.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/grkjnmdtr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gzmqnqyfz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gcnxzmyci.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/ggxcqtgyu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/ggunfxdsw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gkctqibwq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/givkipzam.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gvuunyclq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gjnwvelur.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gkmurypql.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gawofhhwh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/grgqfudzt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gjfxcnoxv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gwbzmyrss.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gigpavqxt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gcgsaprsd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/ggertvmqh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gfmgfalyn.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/godabcgrl.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/goxuwhzja.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gvxyyhptq.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gozvohwkc.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gdbgfbdkj.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gzevfdbip.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/geazpobqi.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gmckohnqr.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gxoqykxbr.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gkhjylsyq.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/ggectyokx.sHtML


<!-- 参考信息 -->