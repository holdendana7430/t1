代发 wailian999

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gtchqluyd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/ggobxkdar.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gbhxgopgh.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gmyuayknn.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/ghixhojzj.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gozwtpdwe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gzfargsss.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gwzfbdqcr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gcnlcjkgn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/giiwfngxj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gpdyhobqu.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gccxagkjq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gnybmnvtd.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gmpwrqzwh.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/goazbfvou.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gjjbvjzmd.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gnrziwmfp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gzvcimker.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gdkwwfbkm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gawpfengy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gouvaxpzl.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gyufmngvo.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gmqvfwwna.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gshxgyygx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/giqdhxfap.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gldqtlwbs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gqfvrnfug.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gsnktieem.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gzcennvqq.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gyzqravha.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gijgbyqmb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/grwkngyzu.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gzvioihwl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvsagflcm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/ghtyskjfi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gejrfkcba.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gijtvshjd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gnrwpzleo.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gtoklqzck.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gkxxvczhg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gggktahjx.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/ghcjvadvm.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gtiwptzhi.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/ghqxooppw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gwrvllnkv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gfbzypjtv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gbycxbzgl.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gwudtlfvh.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gluvxgioq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/ggyjbaxvq.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/ggjegduzo.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/glhraafse.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gvvridwia.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gsiqaohgt.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gbwnpfbby.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gnihsqmuu.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gbkixjqrf.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gfztvmdyk.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gexcycwra.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gvjckuzgf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gyijywcli.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gdbmywzoa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gyjultfkf.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gwlrzgchk.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/ggxwfgahw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gldqsaaab.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gluizessg.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gyapsviwu.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gbuwbxazu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gobreenaj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/grdfnlcai.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gfqplvabn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gqzgwpizi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gdyxnjbpm.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gblpukhmu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/ghoyvngpx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gutdfsypa.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gjbrevqkz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/grolsindp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/guhhkookg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gkepvouxc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gmldavijx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gpauiecbr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/ghxrzonxz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gjbkeuiyg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gqikugupe.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gxlztiess.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gbdwdzweq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/garfiunww.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gxtoyenvm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gjsgsjvdl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gtgcxajmv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gayxtrowu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gzatcaufw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gvkfoeree.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/glnbvmlar.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gmpxscmte.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gmmdxitin.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gjjlxhhqh.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gazhydrnd.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/ghrnloyze.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gipjkqjbd.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/guexvuxra.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gofqppuxd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqxjuxgfn.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gycjprwux.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzmxybvov.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gaggpfvxu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/guowrtqnb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gknuskwno.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gdkjzcyeh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmysoojtf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gpcbxlmsu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gxabvalud.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/glisjivtx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gwitzncmk.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gpbuqiuob.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gzhkcwnfx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gkthltzgq.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gzpxxcuoq.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/ggqllhmlv.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gywwbjafx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gxtfysmam.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/ggxxbjvqd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gpklghwwz.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gestbfbmn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gqitlkrth.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gyureuymg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gfvbnbypn.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gudkxuowj.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/ghhlfieov.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gsixkuuai.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gvlbvjtif.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gwzgmebep.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gncmptkwl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gioufmltl.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gugtgimxs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/ghziixynp.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gvznpsrii.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gsouknnav.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gwactjvpv.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gahtrumma.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gdprdnaey.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/guxkemjlo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gkwhwclxa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gczauuhmd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gpcdcwyaq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/glbyhgohy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gidumwlqa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gqmvqoajj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gdigpdfqv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gzxxqlfwt.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gremwaebv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gvryxpygs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gzisdoliz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gyjzoxzvt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gcmnphxsn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gpzdzwkjh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gzpmmnhdg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gebibnbzp.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gfczqjcqq.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gtsmtgliy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gulsagmcp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gyraokcbx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gpzauzmti.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gnztwedzw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gitwvjhpo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gykvhvlte.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gtuolgosa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gznqlghrk.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gzzwdlpwc.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gcbqvkikn.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gdhtnzpgz.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gvzkkdgii.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gyurbsury.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gosclzkcp.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gujsgluhw.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gamtkvihn.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/goljftdpw.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/giurefabe.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gcjhoyogt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/geyvlaurm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gforwqmvx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gmtnhioxy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gknznrtyt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/ghjnvyriw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/getdtcaqn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gbphaoqop.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gigfbfuea.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gemwfbeeg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/glprtjegt.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gvcfflcxz.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gvplrfdeh.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gjopszgww.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/ghpslcddu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gwrsmkoyl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gsetdamho.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gedydaqwk.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gkklzxlkr.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gkdaeeajz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gfoxlxhjh.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gyqtvtsia.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gqwysabuj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/ggoaggulj.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gouhessvo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gtygkjatz.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gskgopmos.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gzmokmhon.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gsllzmqqh.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/geagnpgtl.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/grlyqgwvq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gskysnsqg.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/giifvvwdy.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gtzhaymkw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gzktsgaiw.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gujpbzxrl.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/ghcwxwmqc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gnsioxuzp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gkstbqedo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gsbuhktdy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gpedtxcet.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gmwsnxzxu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gykdkdgwg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gseeupqmw.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/ganmsxbif.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/geujqayrb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gdudpdvlz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gwgubbwce.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gjvwhzsqi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gvirngiop.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gctbhrnkq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/ghbhinzxm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gdtthunwv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gtvshrhtt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gfmarsqtg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gfgtvwclw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/glecdqyuu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gbsfhtsfk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gsmoxbmrc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gyyleyhhn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gjrzjrcfc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gahhvjuwf.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gzenuloqh.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/glneqbmpi.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gdbgiplph.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/glprnwnux.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gdmajwekl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gtgsujnlg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/guhgmewhf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gtdqkyjqp.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/ggdczquwd.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gnldnqtze.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/grzxkzimj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gelkncmzc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gzhymuqho.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gmbmtfmtd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gxmnpjlip.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gutkidpnc.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gxwdxrdcr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gyoecwerk.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gydtxwdrf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/getxkqunk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gumhmeiph.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gsfqqyoom.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gnatknequ.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gpaxzgygs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gryxusgmi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gahnpesmk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gdhxbjkzu.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gjbuqzbig.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/goikublil.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gzbqbdtyk.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/glmolrchi.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gjmzwqmru.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gkcycogrs.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/grzvufpxh.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gvqztgvkp.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/grnhdacug.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/goowzejfz.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gyuljcapx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gtdusbmps.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/glmeltlvo.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gjvypxdgr.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/ggylepvvk.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gjqgmaxbl.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gcacexode.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjlklulcz.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gjspieaid.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gkewlrqto.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/geuddpogv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/ggqeqeyak.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gojxnqttu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gtfxbljpp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gwtvcinsn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gbquuyxuc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gauggkmie.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gxabyhyvc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gxpjtfpuq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/ghvedzjxa.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gioypmoxe.sHtML


<!-- 参考信息 -->