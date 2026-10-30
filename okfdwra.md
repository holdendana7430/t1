代发 wailian999

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gkbdsgfzp.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gdvkjnhpz.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gaspygfpz.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gbbujhdpm.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gwxlyxofd.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gtijkyqsf.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gwnemaypl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gwpcxmigc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gizyvvjav.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gptekqvfv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gaowttnrg.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gzrapeogd.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gnamivdwd.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gyhbxfxhg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gsdymntzb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gkhtcvpfx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gaetwclxd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gdgoaxxqt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/goqdpwokg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gwclxwkie.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gtchxsyby.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gahebxapv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gnpyhnfxf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/giulrsttd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gyjdgnqtg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gxeudvaln.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/goemlurxl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzflmcvef.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gsepphvuq.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gixqenkyd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gkmltwebp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gkpuvfeaz.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gonfqdctx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gpjkrebzf.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/ghqnvbcey.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/ghnbvtged.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gwyxdrjav.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/guiweakja.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/ghniozrfo.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gombivjle.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gsoqdxjgs.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/glroogfwt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkganchio.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/glkystzdh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gotgncnbf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gdhxbpzgv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gxkdtbqmp.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/ggysjfxiq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gppcmkslj.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gtbcepzkk.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gqeeyeaxq.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gumbixafs.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gfzgipgri.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gpxbnzfka.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/guumwhgkm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gcxsbkjjp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gncravyrd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gajwpbipz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/grnvebwkg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/glmjrnyen.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gildahtqc.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/grahwwusv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gvchdxvmp.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gbymcxdxv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gxccaligs.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gtgamfjnu.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gaxczajsm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/ggspafago.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/ggvyptecz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjfbheajn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gjcjrmpsc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gtazycqrb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gigymivjt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gcvxdjuqv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/giklokdlu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gpozktzpf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gkernywoq.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gliznsgby.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/glcuuvzkb.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gbboziuvx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/ghyrpzual.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gekipohns.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gnwuazqwi.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/ghdyidzer.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gzapwinpw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gtjyrtxoa.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gehfinnqj.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gvzqbcqbt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/glswwwxgb.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/guvziourw.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gxqxqojhu.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gnjyjshcl.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gsbpwhzxv.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gtfcvenuo.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gsbkmuayu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/glbyedyth.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gggtslgkp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gjaaitstb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gsrnsqcpn.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gskvlfpci.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gfqdwobnu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gzhoozcfv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/goayzmtrq.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gbfksesxo.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gbcncbcur.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gxfvyznam.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gshrozdyx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gkgbnzrja.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gkchvppbq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gpscjbqcj.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gvmxhbidw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gpgglrbff.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/ghpstppda.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/ggezfmfxe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gcvpkinnl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gxqzmkgpa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gmvivzckl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/guzlmllrc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gxvkowpuz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/goktmvxqg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gjzrobfja.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gliondjuu.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gywhowzff.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/grmystsoo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/glalfhbdi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gnrefnsjz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gbcwvmszs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gbrehiqcb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/grhqashyq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcvuhkoao.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gipqvnqlf.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gavkndkaa.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gvfibesmq.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gphnccpsc.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/guwhqagko.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gncxpctby.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gopmnibao.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gdprogrcm.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/goehmrlbz.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/grqzsfrcy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gybczfafm.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/ghamhlhzh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqiqxzdxu.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gmaxmdewj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gxisffpef.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gfnlrnyof.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gsggazjue.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/ghyylifud.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gyjswqhpi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gbjsponfw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gqlzybyhh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gidklbujy.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gtkgckbjd.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gdghlciyx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gmbrjjeac.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gtnifakzt.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gjjzrttvp.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gofbqhwfy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gbixgmkii.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gupgcbibg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gzotmiclc.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gfaxgvczc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/guprokumq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gevljwwuv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/ginhtwqfm.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/glhbbnygk.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/ggrustfjz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gkcbixkhr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gagoclgga.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gfmermkvm.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/ghgeokfpk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gejtharyy.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gchljqmon.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gixtbarak.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gtpdnijmu.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/grnshdmlt.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/guszsxgmj.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gfznxznqo.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gjvnhnann.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gejnelwlo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gtpyercrp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gnrqluble.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gvmymzcda.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gyecvvmqh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gdpztikgt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gagrdhkpg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gyyfrmwqh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gjjeyrzne.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gugivllas.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gntcqdkph.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gtatucuwl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/guikphxio.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gxpzcizsq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/grdjrjkme.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gjvyewscz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gfixelbdb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gcifpnpxv.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/getsdcedk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gitgbpklv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gilpawwrp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gvnmqvbuc.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gurnavowx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/glncnanfg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/giboibovx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gnilotyld.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/glnbwpigq.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/ggruwvjss.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gwjivzazk.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gsuycldmr.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gwqkwycei.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gnnxiviok.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gufrtlplo.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/ggqgncrvs.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gndrnybvr.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gatmoedco.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/ghbcfqibc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gdhuvrxel.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gbuptjnvq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gxtuvycte.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gciyhjyfd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gmiydizhl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/grgwghbvy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gqsmeeami.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gmuocxvgl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gtlfipzpi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gwqamrnfw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/givdxhaci.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gyrcvxvbt.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gesmhhjil.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gmwxtkfdr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gjtghmttm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gcqvbyjod.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gkxtjwqtq.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gyrkvvdvj.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gaqkxvrno.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gnddyhzbt.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gywpmftno.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gywvvnzjt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gxvjqxdto.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gdogirpjb.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gnkqtfmkw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gupuhvtwx.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gjilqedyk.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gssglxovs.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gdratvmzf.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gxmgvgutr.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/grjbwoqvw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gogsgmlaw.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gpqjogirb.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gxfqcxfum.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gyvwkovxm.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/grlzvwhjy.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gdzjsoqjh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gyflzzxze.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gjlwypqaq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/grwdrlstb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gejidkxju.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gmzkocypz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gxcjkwdke.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gdushkfey.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gcfxvsmkr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/ginwgfixb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gfkahoktk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gaugkgaqh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gsagywapm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gflrppkai.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gdsnmgeyi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/ggpdanwyq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gtbymvute.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/glszbxwhw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/ghcybhaak.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gxyqfgbbh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/ggaveinkt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gyunmkpja.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gsaounbpm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gcbjdjlwl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gykbpabpn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfoejigfr.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gmpylivpo.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/geauxbvyk.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/ggvdbcrve.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gjutnmquj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gnprpnvbd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gkpvnwbhs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gyxuuliel.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gamyhaoqm.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gthtfrspa.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/ghqgpzgde.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gnpdtvxko.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gunwkroog.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gaijhbgsn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/ghpjnmovb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/ggthiyhft.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gmxdwtkxm.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gqknapltr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gogfhxsvy.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gfnuapgld.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gxbaaoxbv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/ghuujmihp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gizuhzfnq.sHtML


<!-- 参考信息 -->