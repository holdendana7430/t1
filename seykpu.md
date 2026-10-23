代发 wailian999

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3siszvjmk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qmxdzjit.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3kyuutdog.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3kayabzmc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3hvmrxnzq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fhiccuxf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3baopwwgj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lnqxjpym.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3jyayzndu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3kvzqcahy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nojomzxa.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3sseishuj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3egwndvqz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ybhnvkth.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qyiektsa.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ludsvdnf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qvgwfrzo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3bqncmaxv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vfkxsyrf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jruxrrht.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3mjhiowiq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tvnojdzl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tfwzveje.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lxihathp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3eotqjcht.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3sfkhkmqv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3iwhrzoen.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3shywgide.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3muerrdft.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3gemftefw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sfdvvimp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wzbmjwnh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hknkdvyo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bkpzucec.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3browewbj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3shvloume.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ffgqedux.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qnhgtopb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3sfrrwtms.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ontvyuzu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vftgcoxd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3dsnpwdem.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dqfkxfzo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pcsrhzls.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dciqikyr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3bpnsyyhm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3fucuuiah.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3jyxmxkdv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3uqqwsjiu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3yshjxdwy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ieysywgv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3qfifwlqu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ifxgkuiz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lljjkjgc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3inafokcn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xysrfine.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3yvgzumvh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3mwitkkis.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3pxyefcrf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3nynyucta.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tartzubp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3scrgokrw.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3shgidmad.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3oycqvvus.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ebjhijqd.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tzubuamu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nzmofswr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3syoaclhr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3tlzuqjfz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3btfyhloz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3fobagjwr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3qwootpwo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3cguuulsm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3anqralia.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3epmgfnsd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qdatvbax.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ypnhtvev.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uvufhanp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qqedqmzt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qzppaokm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3erfomqxi.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qeczwgiu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3haegskan.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ooxadfvq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kekldrdk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3hcpvcrcc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ffdyqhzi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3gaipofhe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3prhbutua.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3krhewjrv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3cwotsqrz.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3cvvsryaa.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3acnplhbn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ctmzlrst.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qafifjbx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3csrwidcq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tkmsxkvr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3bqiipcfq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ripdeqoe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3vxrbumlr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3szmiyvah.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3uwumuwzj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3kstpsycm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3odyukrzn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gycrubgo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iituoiuq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3gllcmymo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3odiwhqrl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3wmmscrvc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3rpjuzptg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3rgmjplpo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3yflrpneu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ousywesy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cxbzffzv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3pyojaope.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xxljrmrb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3faignpgc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tgdglxmx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dljdwfoy.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xgkkprtn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nzwynwer.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mwluqxzy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3snfehmnl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rdrkrsxa.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3aafsnhzu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hjqzatuj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yjbgkbkg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gnebwumf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjywsdpf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3venoilim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iluqdslb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pcpftmtj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ycjodzzd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kklqutog.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dmyxluvr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xdozpnin.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3uvqnzucy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gguurypo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ntznujvu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3euwljcum.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3qxrxkhzh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kfpdlmgn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3rlvpmifu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dmrikpfi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wxljgwht.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wvzzonnm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rmflvdep.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nwrntknw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3myywelnw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3iqtmwhmg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ksymoyxv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xvjwftni.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3emvgclfa.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ssdodnyd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wqqirfuv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qlanggdo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3bdtmttgy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3avasqcuq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3qclzwabm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3brflrwwl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3fhwxczwm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bywmklwj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3huxcbdeb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yycegrtu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qptxwkno.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3cptejdwf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qjcfhkdi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3mfgaadll.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3kulbkfly.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3qaktmjqa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yypxleor.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oyzofaon.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3imbhcvyj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3whtfuyda.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gfawwurh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bjcbbfju.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3sgkndzig.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hnxzuqhj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ueuqjglg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lytxwqlw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sxvrmwwn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xzjxhggr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kcerwror.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rtbcfunm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ppqzqypd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3lhltgqfq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3zsblqudk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nzggovdg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3derlpnlw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3hrmtervu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3gsfrbqkj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3fehcqpsm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3qrburgio.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3shsapsel.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3jgrssywm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3srbmobab.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3axtdacpx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pexuzmss.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dxfwrgfv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gidzhunm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3abgtggly.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3aspkzskr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ycnhsvue.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3cqpabdyb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3vxywjsph.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3otbadcup.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vxunrhkq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nehewuhd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qraddvje.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3kwktjswq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ngdiwrtz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pxmigfik.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ztypkloy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fwcczbzp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3cxyscczm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jkejjxge.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vubzcnaw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mycggmiu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cbssoxxu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3igbfeyac.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3filhunwj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bqvccvsk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pmanjmvn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tkswcwbo.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oxuuerjc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3epzuhxrn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3msyveiwc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dbxojwdc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qzcfmoti.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kbbndrrj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mkoufbcc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qqnfxuui.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3zsqgtfza.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ipslbbjo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3erqdnxgw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3zjunjyra.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3sphtwqcb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ynxuryma.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3bamstxzw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hiwtjiek.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3wpysmyga.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzchrelg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yextbqsf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3otnnesnr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qaxxsaba.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xysfdcjw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ypdquqfc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3chzwfyem.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3iaepfisv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3fdudecbq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3zoknmoqc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3sszddobp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3yjdnpcwf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gdbzxpdm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ihzdgymh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3uskmfygb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mifxkswr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3imxcsowx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3lwslxgpa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tanzvjdj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qccahvuq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qwlzipao.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3jkhgtxfp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3rnhpbhci.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mrxkgkzr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vnnujhfz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wzdvjjbk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kahgpirj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3blfadiga.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cjnruucn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ptqmvfbc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3srfoxtjw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3osdkicym.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3psosnlbs.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3dwskmagn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jifdtnoz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ctqcbnwy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xckpbfoo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qypkpwcs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3racafhht.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3todpzoie.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3bkvlrrkc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3khmycrze.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3srmnmmsd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vatellow.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3esolrwwr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3akllmiog.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tafyjges.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ybmudznw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gmvhjbtw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pwkgnoxw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nhbnugiu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bqiqjsvu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zktubsxw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3dybbcqrm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xzsejccc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fonffxnu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zogflcuh.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3bavkpbdz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ijqtgyek.html


<!-- 参考信息 -->