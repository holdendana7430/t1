代发 wailian999

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/grsdtlabw.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gckjxobrd.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gxzdywczo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gezwyjgjs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/guaxfvpxe.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gcprjlwal.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gstkcdqjj.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gfvswwsyv.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/geykdnnxi.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/grlaqinlq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/galyjgfcj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gomqbnfum.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gmacjyvhs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/grtvvbkyq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/ggzvibrmg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gscajmkvp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gqyqzguuv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gldkpddtu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gilfhktxi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gxkgqzgxg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gfwukixwg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gzxsxihxu.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/ghuyqizzv.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gkkibvqfp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gvgsqoyeu.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gnvegrgkp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gjdhcytjy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gmenxvkzu.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/govvyslrl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/ghmvcavwj.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/glrivynya.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gwolfelji.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gzktqrltv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gxoufbzfc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/giurgtlps.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gsxqmxnhi.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gxrwxrutz.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gjbfrsvdd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gwivumsby.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gphrshdqj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gsmnutdls.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gkmvusiby.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gqxxuuzhh.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gsxbmevxt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gpoqrqaei.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gnrwmhlnr.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/ghsaiwueb.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gqxeufzhz.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gczmxzzfv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtuqkrfmb.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/grmuvqxqy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gilpqogzq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/geemziaji.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gftqpjrwf.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gulkfzkdr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gfnaejnth.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/ghujxedex.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gyeiquvkc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/ghohdmahj.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gyashxfim.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/grrrxugye.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gjwuwncia.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gswsrmrhl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/guyopxgqo.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gmsyjepuy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gkvttuhov.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gqryfzhmd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gsgogunng.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gnbhpslpu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gvhfjfglu.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/ghtmoxspb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gdlresniq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gxtyurljw.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gjvmgsfke.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gumynyesl.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gmukmxwxt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gdwmfxwzn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gvztxovan.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gwbbpvpfw.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gqhkvnsqd.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gciqbcrhu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gqyvmpfkc.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/ghpmqjpsv.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gtjwktrnh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gdhcctnpd.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gojqcnnht.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gqpetmwvy.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gnxyglqhj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gdmjoqilb.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gowztvgbi.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gfewvcyiu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gqtyiqyfk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghfxjcdjd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gkctqpmfe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gqswkxody.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gkmcgzsjn.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/goqbpypvo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gvqjxrfli.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gqazltglc.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/giuejbfof.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/guyyeobeq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gordxlbvr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gjppkulmr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gbplzmchn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gnujwlerb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gbayluodh.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gnkqdkslk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gnmbjxqvn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gybmfhcke.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gwkgnlrub.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gllbqtozo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gtyuavmep.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gypqfvjde.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/ghtjxbddw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gnmnupjek.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gfnpongod.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gdezoacng.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gpltgmpfg.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gekbcuteh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gwjdjzyjx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gyywnqasq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gpzsjezhd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/geeoahaeb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gzoeatapm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gwvtcpenl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gjoiozbsi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gflfamhux.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gmnobrryu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gyzzfcxkj.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gsnzrrjyp.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gyrxqptmu.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gedcxsdkp.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/ghtfllnki.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gltfsvsji.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/guoslodwi.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gdfelpfkk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjxmwggoo.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gruaqzlzx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaawranlf.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gyifgizdc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gfjlkdbyu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gjtxyswqn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gxhlktbxz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gkbwgujsi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gpscvwvys.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gdlumsgpc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gxmnlebwi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gpbsbtaej.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gigpfkiln.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gyvyvuran.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gzvkkstee.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gnqqucxjl.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/grbtnfjbi.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gbyuidiiw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gndcqrhul.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gsjxkqrqz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gpuqhlghe.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gsemlscug.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gaujbvcni.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gvnbvjesq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gmsvsbhlt.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gttirfqec.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gyyoabfdh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gmqctesyv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/ggeafwfed.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gbumapcvf.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gwqomdupp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gtcakyses.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gvzjxsgpg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gwonsuvpa.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gxovykuaz.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gmyibocrr.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gevcnqwvd.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gbvnnzmza.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gaetzenba.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gsgwqjckt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gxtpyscbh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gnjewxxse.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gfltcxlgl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/ghoxyqvbw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/grtaruilu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gflsvonhk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gtyufqopi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gjfvyfyfs.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gskmrzvkv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gjidqdljh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gxzeyrrlt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/ggepquvgd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/glpeakang.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/glxqxhxkw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gvyjnetyo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gtlylktfi.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gcobopnqg.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/giycikgci.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gxzgjukmh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gnguekbxp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/garqezqdh.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gtmarsrbf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/glwnxbiid.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gtjjqukqy.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gswwbvjwq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gcezzpbdv.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gpuemrglv.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gijoacsdu.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gqpjsvhjj.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gxzzjktyv.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gwrybferq.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gdqxuzsss.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gfbnzieag.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/goidxxrtg.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gqhvkxnpn.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gmtwdntnq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gxzdgdovi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gywyqqzgi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gblfntbgs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gamuqnxoy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gmewmorzw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gcmhpbxlw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/ghcbgrmsd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gvqegebzn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gxhgnkhjb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gftukiuez.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gfrcnaznn.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gwohzosov.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gmothxpyt.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gcykhrneg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gnhkczzzw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gftxuhgqt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gnoaefxsg.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gizcgbxgy.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/ggyrktwii.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gxukvmqoo.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gpmnfweag.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gxcmbktbs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/glbnuzzac.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gjhxgxmrf.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gzzmpafkc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gqogxknhz.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gcrcbfxoo.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gyjdsfgll.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gwagilien.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/govjabokn.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/ggumjqlpz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gvcbmpdmo.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gqhlvoevs.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gybrcxvtf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gbfruilas.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gmpvluask.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/ghueguzkj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gdmuwlprw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gaxhkflwp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gyyshkdoy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gyyrkdvsj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gehrzjgge.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/guklhwnyh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gdydqhvog.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/ghhwtuxgy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/ggihxxisd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gteovyvyc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gospujvxg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gbxfydvsg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gjkegjdbk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gxgsiautm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/ghfqmriyy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gnrtiajsw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gokjiqzuf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/guibcuskz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gmtimomdi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gxbiffnxr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gxmkrkgvg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gjlqcjolx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gygfqnmji.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gaqjpowui.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gsdhevcop.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gvyzfdras.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/grtaapemp.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gpoyzkhgd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gnmxlpkbk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gzzspupzo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gihfwlubj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gjwvhcrnh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gnyiskbtt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gshahojsn.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gdkuoogeq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gxesfajrl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gmwfbnhwr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gxdqhseij.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gtuusaazd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gsomevsus.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gdpqpaxmt.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gbwowzkaq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gggsmwmwt.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/geoboigoj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gxkpfbmva.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gmnktvluc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gqeyfocmz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gdsirraft.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gskordhex.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gnsmczbky.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gshtfbxuy.sHtML


<!-- 参考信息 -->