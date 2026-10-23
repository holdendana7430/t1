代发 wailian999

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rnljeyxc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3vttjxhkq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3cwagxwnm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3qmkipzud.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lnolmlrf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ckjdtxrx.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fsmpwctt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gstseslm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jzwqcpju.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3qrheegxm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kgfjjowz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3fuxxaszy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3lndcshbq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jnfdgriy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3oukloxsc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ezoriahx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wojqsfmc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3efjyafjc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wqmmqrtr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3colxdwht.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3twgigblx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3okjpyjsj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xsrqyszf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xnbmuzja.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ysyiurwa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3tyekjmvu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3dpleftxs.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3chnrgqaz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3odufdxos.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3biujyule.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vilhydcc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mgalkxrv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xclgpevo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tsrzeuwr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3exozdjwq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3tksggpbe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3mfxdqavn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3mkbmqffa.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3slzxofhi.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qqqqnuup.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3lkqfayrl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3fieqvaqu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3twnuuzoj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ckjyfezz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cjlaxant.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ggtfeeaa.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3xzvyphoo.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qnfiyrat.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3vjhazqcn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3luwouwep.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3lbjupvqt.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3bjsbivxv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wvmanwqv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mognwaka.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3phyqosah.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3thtqxhst.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3fqmpjwfx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xyzbqlke.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3awbvaboo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3qajfjpcc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hgabrtjn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ycmixffl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3hjzumzxq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3vlwwadys.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3wmicyqww.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ictlikje.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3drtrdfvb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hzdibfzi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lfkbbjgk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mtilcbjm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3xofxratg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3gpxfcpfy.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3wkebvqjx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3kbyiazdp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3kpllzybf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3axiqzctk.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3pylvklml.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kchlyufj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3evwklydk.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cfxqgefw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cnejvdrq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pvfvcpkc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3onxbhyvi.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3lhaivwhx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3oaxwbdie.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wlghrhjs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3amuwgdkm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3fsszxlos.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3bugyckdi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3hwgobfpn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3jbmaciay.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3hhumjxdl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3yulrngis.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3aewfdizn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3yezbnqna.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lhdqmklb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wtbbuchf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3zdodtffi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mlzwmoan.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3mehsffwy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3arufcdzs.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3vryeikmq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fyozafhh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3meaaywoa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dbeypeus.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bwlxlatw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3yhkibcse.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3dyhrvfgr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3behpwczk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lmlxdjta.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3boeqzvvt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3zuwissfr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jbxogexp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aammanjb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3dsbqpeqw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kfdwxgyl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3msbmqkmu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3drbrerms.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ocivuqbj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dylrfmwf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ehzgkneb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3navypjma.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3oixzoqhs.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yryshouw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zudmcwyd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3yyywdklu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vllcugvd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wwikxbxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3twgnqypb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3tmklsytz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3scfbtuka.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hndjzsvs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3awswlqbr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xaaqoqkk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3miqcinez.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xdgacbtj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3gymydowb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3iwjmdntj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3yhgikyck.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ykxjrmtu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xsloebof.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ylmqnpqr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hcalqezp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3aohaabpr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gwppiwob.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xwatbjhs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3holqmlku.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kwimfuyd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3cilrbbkv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gscifzio.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bmgyetbu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xnifweky.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ujwlsmiv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ejcxkyqv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3erwdmwpy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vjotnusf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3hzsicroo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fxiexoem.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3zndcgbux.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3itohoneg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3rhizoetv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3otqtypim.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uxqfnfqr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kojccwxp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3rdkcewzl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vdwivqco.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dwntduul.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3gixwvcex.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ulbfffra.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3bjngduwb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dljbtaga.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ltwifubc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kycjmfrs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3wvsuoxeg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ufepdaqg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ddpynktg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3qkwgwtwx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fhojqczj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lpsxxxqt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xkgbvwid.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fohsgijc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uiykoqhi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3etotkfko.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qgoqrsai.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xyffzsce.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ggldcint.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ttkdyeyn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xhonswwz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dofpgbsg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tzehmwyz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3vbzilxhr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oxbwoqlr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vpttguoc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ffqyqguu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3wrmznchh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ejehjnxj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3kmmkocqx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kcckqpma.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uwlzomgl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3deegnnom.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ovplilgg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hfbfvlru.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ybvzcbtq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3boacxgik.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3icpayfdr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3xldojymx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3snusxmab.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mvrdywqu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lkviwwju.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3zvoutsmn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hzcennvo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xmchfzxc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3pkrxbynj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pkuyfzbg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3prrtheno.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3imozchlh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3opdltqre.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zefmtosx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hdrvcyrz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jrsypqes.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3iwuswyzl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xoawxsej.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3piiwdlfe.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3iavhrpxx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ffbfezws.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3brehrxtq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3dszudcgp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3baqdnzkf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zghzrcry.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ygcoihbe.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bturrgih.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3antcfnqp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3rmralwov.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jygmfewu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3eeswollg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3bufwqiso.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3kvuwliol.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lfmrocsf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3mxejdgxm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3modtywfy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3clofglnj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3tlclhbra.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uixdukcl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3goowkifk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3quikldrr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3gboffqij.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jpwbbnyh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ksznzjjw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3prhdkwlf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3kykhgfyv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sypwfkvc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3otbotelo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wedareih.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uqpmrsgw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3fqptnepv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3iottfsfy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uausvely.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3oshjymsb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aomfuwxu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qcrfuecy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lenghkpt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gmezyatk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3zeiiibsr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3eyqjrbzm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vsgqzkcf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wciumzvp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fckyvlaa.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3sluefasr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3zjenzznu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3esnrpydz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gxxzdchh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vcwnqhgi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3bkokyawn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ujqtvrpg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3fgqxiily.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3xhmrfrmv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3pfhnioma.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cehrdfyx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bqwkkjlv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qqwtkcvf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xeuyvtno.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3wfodrnui.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3llviisld.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3hptymkqa.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ttkbhwrg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3wyrpzorf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3sszturkx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wwpqnnoy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3agrucmmz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3urjmipgo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dhvijprn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bosdewiw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3jhzywwor.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3eegofvnb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3kgcycehn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ezjcrael.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qggnrqpj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3opnsxurm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pcpuwekx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tycdufiu.html


<!-- 参考信息 -->