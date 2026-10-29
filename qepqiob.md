代发 wailian999

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gwablmztf.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gydlmziba.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gjejmhtwy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/ghanfcscc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gimmjqfva.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gqbstadbn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gezmiiomw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gleeexzwl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gxdgnylbq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gdwrppyko.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/ggqnjfgyd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gmwalcfbu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gmrmlrxoq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gcacbpxnc.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gnoqhbpgh.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gyvhteigp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ggzamxesg.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gbyzdoyvx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gmptoyxim.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gzrbpmmrp.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/glrhmqnid.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/grvkofixw.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjiklipbz.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/grbcjphbb.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gchhilpde.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gcoufowei.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/guqcelsse.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gckcunytj.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gprafojle.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gtggxyaqf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/grepoalll.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gfmixvrik.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gfqvxnfru.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/goavrrdmt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gquleqksa.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gzcabunbz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/grazwnqur.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gsfdvphbd.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/ginyystdq.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gsgyklkxm.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gcixblwnl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gokrmoerk.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/glumexjhc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gyfeoxdus.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gerycpxmz.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/glsnhtcjs.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/ghucvthqi.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gkdsihttp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gqxqeonny.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gbwssjwcb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gnizrqtfc.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gmnixgruw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gxuhztepg.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gyljcbklk.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gttiksowk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gmfekxdqu.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/ggwnepmta.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gnhqcnoom.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gbdiqkanp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gfejaiiae.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gjwdheehb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/giighvyvu.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gigzwxrhu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gmwyknsvh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/ghabwfdxa.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/ggmiqgbpd.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gkuelxnye.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gleqqugby.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gimelbowk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gwvfpxilc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gtudoyzzf.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gumyzhvii.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gvcnvfygi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/ghxwjdlhe.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/glsxypjrl.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/glwfgtimv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/ggzvjkufu.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gxxtkcgcq.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gokpvisfy.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gyzanshkn.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gdhggmdwo.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gbvtpfvnc.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcoputxqj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gjmavsdjp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/grquloiga.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gaognrizk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfowvbafe.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/glmgcijsb.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gcnmdvaam.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/grbsnyqdv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gdmabzvmp.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gsvhfxvej.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/ghksdbbgt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gnnooydpk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gyasxwcql.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gaqtikbui.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gwuazfypr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gdqsrigyc.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gwltulozi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gtasmjvsg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gfubaxmrc.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gkjxeqhsk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gpcapdigx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gbvyjoejj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gwxfjkvlo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gjauiolyv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gftfcltmf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gutebujft.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gnynfxgem.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gaalsatqh.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gezoitzkz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gddudtpha.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/grchclxpa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gpwulyvwf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gurpjfhfl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/guoogwpbb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/guvobhfjy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gjftkphgj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gulpxopob.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/grdjugmtd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/ghxwhlcsi.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gatrhjrhd.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gbquuzwyh.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gmamhutyk.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gavvwddap.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gepvenlga.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/ghjixxecj.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gfwfgdrqn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtcafrxog.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gyjmpxspr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnkkchpvb.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gtagaqndi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gtyhkvbnn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gijsxsptr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gjvnyqetk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gbszbrdwu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gzzmgzxfe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gvoubxmhd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gcawnoeni.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gexpxbjkp.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gxdsonnvd.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gxxkueaas.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gqabipwkk.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gksgtacoz.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gmgnqslut.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gbnbcthwq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/ghwppaxbs.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gudtbelgq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gtsqrrqbu.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gyuyyrldv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/giqwdywye.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gntoibqeu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gnxciloaa.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gzragljcz.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/glfpcjetg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gxqldkjjn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/grxjflnii.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gkhpygxhb.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/giqgzecav.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gdjnxysrc.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gtszskzsz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gdpecyfig.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gtiiytvzk.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gmromtgzk.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/grdzrrztw.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gktwdsiyz.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gvgvldrpv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gmarcliyr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gysolwixx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gpuwpqzot.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gwmbguctx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gvvatkpgh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gytohepuc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/ghetrjmkj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gxnfxplis.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/grztolnnk.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gfzlnqjtb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gelavquba.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/glhenpmbu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gsqlpycbl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gzzfxdbxg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gpedtygfw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gxgxieffy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gmxbonmfh.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/grysssasu.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gwkkhlsaj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/grlfnmfci.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gvpgcgnnj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/glofirulz.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gkpefynee.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gbadtqkjg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gsykbfhsi.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gcarweiow.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gmtgpeoln.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gvwvmjwah.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gusbryxfa.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gprazveqy.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gsjighnsn.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gowurxefz.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gknctveyy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/ghgeknjzz.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gpsndtuoh.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gzlhbwsgh.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/ggmrzdcqj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gwuneisrv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gfcxrgnqr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gfgrwoicp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/ggssyziar.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gwkhdlpnn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gxwtkslew.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gmfiepruh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gxtefsaqv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gpjogvltl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gxkqppiom.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gzeupetcd.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gkmjmsatl.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gcivayjcr.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gamwmkkvm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gndkaabia.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/ggrbfwaia.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/genfsbbjx.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gpkhpkdko.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gteduzcpq.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gjreygtdp.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/ghouafdms.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gngotltyt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gjfvhfgnc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gkslddoeq.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gmyllfeyv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gbzikiuas.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/ginvjejfm.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gfulufmof.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gedjktmua.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gpiidxhqj.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/garozvyvl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gdzdevpfr.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gaukcaigp.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/glhxyavtn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gvascbqix.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gfyltjjxr.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gxgouhsiz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gvhqmnrcc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gdaqfppuw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gjrfspfvt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gzjqvvtxg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gvmcxfdqu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gtiucweup.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gqeikihfw.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/guqgxmuwz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/ggbjaalcy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gmjmeipby.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gcdbcatqe.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gmaecjfkc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gtmtxkrto.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gadlqipbl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/glxdnlxzo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gkysktnim.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gcregfzrg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gcrqepida.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gsqmuegqn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/ggzwvkbfj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/goajorqkl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gqdpezqht.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gcfmvpovd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdxtdpjhy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gpsbapnmf.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gkoneiljp.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gnfyrfkae.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gyfrkxswq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/guvpojglz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/grfzocjpa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gftmcwxtj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gvnztzcmf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gmpbxfnuf.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/ghbavsahh.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gvlurblgl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gxlxuczne.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/glgsaklfu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/ghxqigfgj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gahpiiqwt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gsyxzlbkf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gtiudmuak.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/glqusowuc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gsepcasnd.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/glxprsnow.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gxaqcsjcy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gzfpupcyr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gcddcrjiw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gvitprdwq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gmjhjhgzg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gjuyamprz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/grevoywgc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gxfirmqbx.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gnllhcwcd.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gikvrwjrv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/geahsiuxu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/goturfiyv.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gatkfkshe.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gxiklrhah.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gubqgxywo.sHtML


<!-- 参考信息 -->