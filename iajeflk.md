代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/glrkuefob.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gjvdwwubl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gzcpoappf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/guowcomrb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gkxigoral.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gjdaljkoe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gmazwxtnr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gwlxnlhnh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gdnpylpwe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gsotlkpvs.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gpuopwhyk.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/grchxeeyq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/grhsojlvh.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gkhfwvcjh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gxbhwvkia.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gicofqdjy.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/garkkfecb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gjlbmgjax.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gchpodfpu.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gcwwrtvnc.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gasaicpzp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gktubcifd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gblepnhyv.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gjosanxde.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gmvaoghkl.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gjbifrdrr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gbmlnpjdj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/grqpcjirk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gfwturnjj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/ggrhbpgxk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gjomycurs.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gkkfxqdte.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gngwdjpbq.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gmeogddhz.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/geixnnmuv.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/glynloloo.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gqlsmqnbf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/ggmkmidgl.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjpzrffha.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/goekcfvbu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gicytiqxr.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gnwohzaie.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gslfrcdgi.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gvagblwam.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gplccqmry.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gaknfhikn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gltlixqqw.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gyswhabpb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gctsqcwzf.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gqtnywbst.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gdadbwewn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gwfseyjwj.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gzwlotbha.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gwgmetlyt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gkyzchduf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gpetdumff.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gncabfyjo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gasesnuyx.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gdhcyrdbp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gnutzsjxh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gtwwhbfor.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gcxcyikea.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gnqltadhu.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gxkdodfsi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gjmsdzycj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/glpdbknmz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gksjvzwbb.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gnhrotiub.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/glkhfzcyw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gtzvqjucv.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gxsainqju.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gqplypjfj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gdnzsltkm.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gswhutfnd.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gdsoupjra.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gvmcvtaxv.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gcpcpmoie.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gobgjvdgg.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gnnzvmsux.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/goflkwrkx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gpzgtkbuz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gvpcslalq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/glweezoqu.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gnpukgcqd.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gpanceadw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gqvkgonza.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/ghakjuust.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gbqxcfhiv.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gpkfkzgce.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gdpwvxngx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gdsaiakpp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gpetdfhrw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gbqrarmrl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gmnwelmgj.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gqazzawsd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gduigekwn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gnimvwknz.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gvcszdvrj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gcbboghlf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gblgjyosw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gtjtlgnrs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gclfwmdzc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gphpoysqs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gktaaqkuy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gizqezsgh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gzompasgv.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gahaajckh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/grbyrwlth.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/geuoawpij.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gmqthhfji.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gccpeensc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gaewrlrge.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gdasixogi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gewiwpqzw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gjrmmxcwg.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gprcuvrvs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gbdmotjti.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/giusovrsa.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gcfxrlliv.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gkoshrbmy.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gbivrudjk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gbmbtatnm.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gzveozbsb.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gyidtruzi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfkctinsg.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gdvdxgeka.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gktglpcyd.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gtyhkkgiv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gbljfahkp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gleentqkz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gazmtxsgj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gppeljmyb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gxrlsdyir.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gpwsejahg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gdqzcirfu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gvygjrjwt.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/ggescnqpk.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gausghjvo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gjrjxxnmj.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gzscnsthj.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gbjmpgmyl.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gldibyrrb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gzypqmgcy.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gxttdeigy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/grjcvfjnc.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gvvhfzqpg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gpfallhjx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gsoizgouz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/grybadkkv.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gnppxggvs.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/giqqgamly.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gypbzrmbj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gnqffznzj.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gogwrsksy.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gnynoshlw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gegcrkbpd.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gwnuyfvgk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gwtduhkud.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gjnqhxedq.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gxmbgupxj.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gkzvwglrv.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gvjtcqynx.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gdekoiqfg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gyybbjquy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gpgibrktl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/guuaiisik.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gukyakvcu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/ggjqhtags.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gkrbaiynm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gmuqfjxeh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gephgqivz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/grwxweevc.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gwtmdkkky.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/grncshkoj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gunqhmsdl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gvmizoijt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/geogvcltj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ghofkapwl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gwllcivbc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gomytnajo.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gascxyibu.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gzgcwfbex.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gbjjdmhhn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gqckigvmv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gdzwbcdow.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gynrjezkq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gpkddtsoz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/ghfgqjvjo.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gxirtdrmv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gbvkzpmqv.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gxvycqkcc.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gocomwhmz.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/goreerzjn.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/ggqpldabi.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gibjebcgx.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/glkddqvwt.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/glsauhbgz.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gwqaifcnh.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/galzbrfor.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gkknsdhzc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/ghflbjoue.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gzrvmwupt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gazprusqx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gslminsfe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gabomoggn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gyukzmohc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gncmzszhe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gtcvgjnbc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/ggjraaphe.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/glyedpwtf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gsyamxuzy.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gqxtndptb.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gmgullchr.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/ggswxphwg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gomgtkjne.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gzcimdmdx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gmkmoeuhr.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/ggxwnrwqj.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gtrnmwzky.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gzdvyzkct.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gbsryrolq.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gqtmgdtav.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/glbwfnxzb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gffpdnkys.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gpsqvjcyf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gvbsewxkh.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gkbbkiakh.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/galfedfif.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gqwougfuz.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gfvbbkaht.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gfikbpdis.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gqyywygik.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gsjhjochs.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gcibjsdpz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gosliexva.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gxinoddhm.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gkqvrcpbp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gthruhgti.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gkbbcraiy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/graketmcz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gtooptulu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gvyygkwvz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/grdhjjsmo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gvezpxmyd.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gzzwbjdcb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gdpidbhkh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gpmcfjelu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gqqayjitz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gviacpixf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gfxxktpjl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/grnlgaidq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gkmnfpblx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gqflvecjc.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gkuvyxmkz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/guaqplruj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gogzcgkap.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gqaythgru.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gtwtounqj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gkzrdttmo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gnyqyrzeo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gkohyktqj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gwjekfxex.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gsouhbuny.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gmzwkyjmo.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/guropgjsy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gkwerodsn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gixleuzne.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gikeiegcj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gdufqqsvq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gkxhtihbk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/ghfzzglzc.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gtkseldas.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gqaisiqqr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gxlthgmhh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gvhdawpjb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/ggrwivolk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gthmpoctr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gopbjtxye.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gqosuegoa.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gcwfdbffk.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/glvmhhtdm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gmotrdwhf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gcuyquvuz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gncstsfdr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gojynlvdx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gaivtmnfh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gfuncuvur.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/guuibwmdl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gclyndrkz.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gtwdccnju.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/guarlvdum.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gygetkkth.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gcepvzlqa.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gmplhqpfl.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gsxibcdhd.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gtaekespk.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/grkfbdraq.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gfdzcyftk.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gbipozixv.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gqhuojmkt.sHtML


<!-- 参考信息 -->