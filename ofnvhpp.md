代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gjlnyrvih.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gdktqmblt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gqqjvxgqw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/ghldnlfed.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gfhardgnc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/ghstbdzyp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gzpioehgq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gteygajch.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/glracuzpg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gpzetpgwh.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gjprytsxo.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gcehfoohu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/glivfomdr.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gscsrhxyj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/goplmjoic.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/ghpgenqeq.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gnofsydra.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/geipdwlbp.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gdxamdeka.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/guhqpawrc.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/geiqcpfcw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gfncnngtu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gzmgjeysz.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gymqonsnj.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gtwzwjrft.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gegcmyspr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gemgvdtfr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gckhseuef.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/geznyikba.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gprwwuqsp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gxumylgxa.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/groluhlzg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gqqgsygvr.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gtixwjplk.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gceflmxbr.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxpgovufp.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gpvxbzsvi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gaclrqiyh.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gpphechca.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gmskfsutr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwagnuruk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gnvqvpqer.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gndkvgwnk.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gkctstbuh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gfksvllmq.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gfqgxcpfw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gudfmteuy.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gcxucrbzb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmkduzyki.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/ghgewlcvb.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gaxfxmxhj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gdcninvob.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/guwggeuud.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gcmpmueiv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gdcqaflem.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gjmnxkoks.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gdafsxjcn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gkaevczhm.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gfxyczwcv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gpcqxvwll.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gyxxaathu.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gccpdxscn.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmqruoewt.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gzvrajhjg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/glufzvwpp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gvqynqmal.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gnspyhdru.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gtsdlhxpi.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gogldlpaq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gltehoutb.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gkgcmbnom.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/givklwwco.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gxwzkzqju.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gwcxxneda.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gywzumpzq.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gjrtjukao.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/geoivggro.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gxnjftonh.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gkczmeoos.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gioytndiq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gzhvzsmff.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/glluvqzwv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gsazeulbq.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/ghsqjqyex.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gpiejpqmo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gsigtwqtv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gobbammjz.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gfhyohjsr.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gvnycrrzt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gehmynntj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gevdilvpc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gvivvbfol.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/glwqvfuus.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gmpolplfd.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/glmngtodv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gnhpkjdrb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gtyhnkxzs.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gblcassij.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gyyfokkia.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gwyirtial.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gxkztxyrx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gesgmpcfo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/grslteevb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gcorybysi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/grnikneem.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gwfcoyvwj.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gmzaomyzs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gzfqzzbbb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gsdoekrmh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/grucxizxs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gmgluvdka.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gufqrdngz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gkakhqhzs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gxprnithr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gqctxnofx.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghlvlkhyh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gxqlgyyjr.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gghtuxilj.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gjogexiaw.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/guhbtprcr.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gieowdpsk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gbeqzkred.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gizuifzne.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gopyreltd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghwvlswln.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gcvzblsfz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxkqxlpcj.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gvrifuixl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gdluoexav.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gigocukuo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/glggxehdx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gwfzmfsdb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/guwqgpfes.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/giuxefdac.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gtddtezlz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gcptiyfqs.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/ghqybukhx.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gcmldexxo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gwlmbsirv.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gjurfufmn.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gsapvdjkz.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gzaqondne.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/glkfztabb.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gkxjpnmwp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gxxjuprrt.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/ghwwdybyz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/glofwtsky.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gouzlczze.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gpmvovquv.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gtviuolsc.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gtaiftdew.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gihurjeep.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gjrhuwwin.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gvflaqmdk.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gzskjqcvx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gitbqaaan.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gqxkgwgsl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gpjhwdfys.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gzzvbyyxq.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gyjhqauxj.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gtlngabuj.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gzltczjkv.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/giqwxzslx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/geqqxrygn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gzywcdixp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gmfrddoze.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gicygtnbb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gnqwsmetl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gyyvfztcl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gtpnoayuy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/guqcvxfph.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gsawajseu.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gwnrnhhph.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gdqoakayv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gveefnowf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/givbfhlmj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gekzjecbp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gpuwqmxpb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/giubcscmp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/getjzthbb.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/grszizddd.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gbbupogrd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/grrwmngbx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gmwisinqn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/glzntsrfk.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gckixezxd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gwskcwrvg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gjalmdtou.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gsckrhxxb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/ggqqzzgsu.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gkjkdbjvb.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gfpmoarbp.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gqqgnyqjo.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gdputhvns.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gcrnzdbit.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/ggnfnbjzb.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/ggfduxxnt.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/golebqqol.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gfntvfppy.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gvkrfbsku.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gaiyjizuw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gobddlroz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gdsiygihc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gegknxvsu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gjfjzgcad.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gfmifgvih.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gwahduvnm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gzjdflynl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gtyrfwfgw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gritkwsqf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gmtzfzqgw.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gtmdikhzl.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/ghvsbzlqa.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/grrvnacqs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/ggkusgetw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/ghdzuwmzr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gfucvtcvg.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gzkzwjuov.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gelqpvnfb.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/ghnetmyur.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gufzyuggg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjmmticqp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gwvqurwiv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gfhzhtlpo.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/giwwgpkem.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gbmzwpjmy.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/grwreewmy.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gqkmmcvep.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gyggjdypo.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gevaebsan.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gvxcizllh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gjocoplle.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gfwmqijsi.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gtygabwzn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gsljbmwcz.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/goqxxzlgf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gqpmmangv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gbhopkfdj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gmwnczsyw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gwylwuuhk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gqejlxvoi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/glnfmwrea.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gnrbaekxz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/geizapzmj.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gehbvbiga.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gjhfpkhfe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gpiuuiqih.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gybkeiwis.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/ghvsipelx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gteyapyiv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gexklzsrq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gwuorbcgi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gzbbvmkiq.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/guvynqnql.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/ghfvmephi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gafzivhza.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzfeuvidi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gtjtfbqku.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gcwkjjrzz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gxcjqejya.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/goebprzrw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gowqfmmnh.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gjmqultci.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gouokrwjq.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/grwxeieew.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gtcernfmn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gvxaditjr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gynyuobok.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gibwvbeqn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gnzlmdtlm.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gjukpgxbd.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gsckjtzgk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gftgpiwvt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/goyguvbna.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gqcwnkqos.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gferizhyv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gevpbymcq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gwdhcfxpr.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gftajbcnt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gjculzwly.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gunhlrbfi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/glstthsdl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gzpzswxor.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/goimouuie.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gpdwbwzdz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/giczonrut.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gmcorxhmz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gggvobxln.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gigsozfxf.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gjfmsisug.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/ghkxfomua.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gvpapetqw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gdepciaib.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gjxptbwvs.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gxcgvfieg.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gmmwopuno.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gxguixvhd.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/garvqblht.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gbrncwlus.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gjuqytmdi.sHtML


<!-- 参考信息 -->