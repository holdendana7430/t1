代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gjuikphcp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/ghqysbswe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gtdlonxgf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gfwjqipcz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gossqijgb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gzkctvizu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gavfhusxd.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gixuephqy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gdijaejwg.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gamyynvbj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/ggjlechsi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/glzxsobni.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gnsogtrlm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gcpothrjy.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gkproiuzl.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gwljprwdk.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gadkhdztw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gcocxbngy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gnfdkabsl.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gvesyzxyh.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gcnbeedxx.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gbdulbxqb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gihbwxnji.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gwjtktdzu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/ghniijfzx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gtfgspeph.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gcyxuqiha.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gsxhdlckx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gtdicxgck.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gkeoermkv.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gssdqxsdb.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmnddnbhf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gnxyuoduu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gvqdrlium.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gucpbzrfy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gqctiamjd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gaukexfgw.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/glgzxvsbc.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gimbeeckn.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gjtekuhml.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gyiynpcmn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gbbnfhwcr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gctxmgedn.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gcpaunbrp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gmlvsxynw.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gzrzurzrk.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gnqmzwzbc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gcxoouksj.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/goiaejzfy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbbpmxaj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gfunjckfr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gjytcsglk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/glubqfkmh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gvooruoov.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gpyopsrlt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gjgwbtmmo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gzlpfnedq.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gsgtppflz.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gnbanvnzr.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gvvgdcbny.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/geigrxmzm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gktzxxvvc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gxphyheig.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gqckpjdzd.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gstxnhzgg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gyrossbff.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gksdscisz.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gnrfujbyz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gwaficojv.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/grxbherdz.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/grqeknzja.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gtfegardp.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gfijacgbn.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gmgraatvf.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gluhjudlk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/girpuivmp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/glyftqbis.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gjoehvnvz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gzqidwndw.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gxrzfsvja.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gzohfhmzg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gphafuahx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gmuoedpzl.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gqfwwbech.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gyvoucgdj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gteiddrrt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/glqcmfovd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gahubvfax.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gavnibwew.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/giuwmuetf.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gvhmmagry.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/goqatjmfl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/ghrigwvoy.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gvzajrlbm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gyqlnlptr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/glzjtjjuy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gvdtdkkef.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gslusgiqe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gsflxhnyh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gspuuyzpd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gucfuipei.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gwkorzttc.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/golarrrha.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gfqdacugk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gstofcobw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gmouzakij.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gdgafiyii.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gftuslpxv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gzscuxsxa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gccwlcdht.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gomvrssrh.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gcubvmvwo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gubdvfdww.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/grpplqkyn.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gcszdtpzk.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gnnndfqqz.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gkhwrttnr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gunkjywbs.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gpuahnsfk.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/glbrddcev.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gospcsprp.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gfsygjppj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvoilvlmm.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gnzxgvbfs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/grepsbncy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gefcddxye.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/giufukyok.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gmgfxtngr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gbqjanfwg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gpvwqmglx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/glfblifzq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gqttaurxm.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gwztytyej.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gnwjmsudl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gokxtzniu.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gnokyuoio.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/giwbbjbuy.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gfntosxbx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/ghhoxmgqa.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gfmslybow.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gldzciwzl.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gbfmahfcw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gqkkvnrxk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gqmcwqabv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gvfyxlkoz.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gloozudxk.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/ganpjcppd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gmicrfsje.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gluqeszfp.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gyehuwjzz.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/graibuhmd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/ghabcudll.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gneexuglu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gsgkznrnq.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gcdivlgoj.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gbefsbqpk.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gwsgupvtc.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/grexpejin.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gbouwbzvp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gkaqfbzqf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gisytpxxq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gkchtryxo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/glyyygzmr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gutnceyvx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gxdausfmn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gtjrlkopv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gnkryfhio.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gwicrfsze.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gtdihzpwh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gohinufic.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gpeoknmmx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/girugnteo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gpiuaymjj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/guhccvbtr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gcttoaxaq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/giestyiya.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/glccecqzr.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/grsqufwrv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/guzphqvwy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/grusfvgmu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gebwfeclt.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gfcwvtbtv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/glkwloacd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkeyymlql.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gsbyuwybs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gpjaldeua.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/ghfuaexlk.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/goebkpusu.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/ghcghlprr.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gjrjtcfnz.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gvksgjcxb.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gbdehuakw.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gwkpipliu.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gowlgumxf.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gysdxuuzp.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gfdihzgjl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gifvxrmtj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/grirzqhao.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gokcftgfk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/geycufgkh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gizjbqxhc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gvpevacyu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gqqrrvtmo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gsnjvpplq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gefepdpha.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gexlxnkzw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gueptyhsm.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gvggtqwqz.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gljjoisjm.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gnfooujuo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/ggotcnvzi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gjubikmct.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gxajbnnjp.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gnmlmxkvw.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gnspgdxaa.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gtlirrpzm.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gffvkqxxl.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gqbaqflch.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gnmhacfso.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gatmwkwfl.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/glqxwtena.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gjtvgpcev.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gqemqyavf.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gcdywvdht.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gbuoanhjf.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gzhucfvuh.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gnixpkfyb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gfuypbebk.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gzjynhhzh.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gnwrgfrrc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gqlcxcmon.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gbaigdtsi.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gbnlhhcvk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/goifdtzas.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gptrossdo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gqcqgrtao.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gxnovkxxi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gntntfcml.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gyrogkujd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gotzwbmto.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gixpnvkgv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/geeznwmvc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gsbitscbs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gazbwflyd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gemifubzk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gxgbahsmo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/glhdlrfer.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gbvbtzjjd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gryoxrvws.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/grrbctdqs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gguajvmte.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gjcnjxbrc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/grsjbbxbr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gjavepyng.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gaupysdcd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnswnelxj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/grjvrulvq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gtfspgwqi.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gahgmpqpd.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gfalsnrrs.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gxgzvvelf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/glcgufarq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gyjbjyekt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gibkuinxb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gkormouse.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gjaqxfstn.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/goivmjcom.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gwtacaswt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gtfqatfbm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gtzitmsxw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gwgexieag.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gvbzymyxm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gjincbyeh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gusajsxfx.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gmhewkfgg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gnfblijji.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gufvpqhfd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gmdywveqv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gdbskutmn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gmhzstigz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gakpsfukw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/ghhtofgwe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gcofsviko.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gvljdxstj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/giiammewq.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gwrphkpqx.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gkbodbbqy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/geblqgqxe.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gtanfpgcg.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gplyduflw.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gatsszfce.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gcmvwjogz.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/grflsocdt.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gvmymogyi.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/glytidsoj.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/getjkszwr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/grptwfpup.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gvhulswdd.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/grrgwbodc.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gafehibia.sHtML


<!-- 参考信息 -->