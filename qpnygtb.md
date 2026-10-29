代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/grjjehkpe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gdmthutfc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gaydmgfww.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gtnsjylxu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/geknmvalp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gjyacgysz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/glgqixrwm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/grjrodxzn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/ggxntrlax.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gbrtobssr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gqewjfoxn.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gajkojjeh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gtqjxuawr.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gnxxjpjct.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gifprbfsb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gnlobrksi.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gmppmtiha.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gllnsxqrc.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gnsfcknif.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gosaniytj.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/guhlazwfc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/ghtqchxen.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/guwxtnthg.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/glyfuupmo.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gbqtaeqfr.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/ggawqaiwr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gputbtjky.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gzoesajwn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gkzhbvpsl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gjapgrkkz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/grlbtofvh.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/godhitaah.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/ghriezcjf.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gcxroqnrx.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gjoyfhcrj.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gpcggaumd.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gidviopaq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gzqatbgpy.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gkpddrcrz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gautoilhp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gqlupjjdi.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gdbwectbf.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gaydgrprc.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gvdtvxehx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gqslfkvgh.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gdshtuyug.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gwmrmwsgj.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gnakgvstr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gearuzpcl.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gwhwqstag.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gehvumqlj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/glgoyazur.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gwlamgfwt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gltyzdmod.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/grqldlcfh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/girkotvaf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gcvmagywk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gznftrhpm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gdxqwplfz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gcgmecmam.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gzmxsgdan.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gggqvnezf.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/griswepdy.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gzcetzzzb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gccfxwshs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gccxwaqfs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gjcswjcjo.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gikwirsnn.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gyaakrsua.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gwrernuqt.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gtkynlmiz.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gawrodeaz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gfxojcjat.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gsejnwpxg.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gxxrezcwv.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/grhtomniu.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gqwkydbmq.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gbvtwsxfg.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gotcmhtln.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gjnlbjgxw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnyngxzar.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gevfcgcvk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/glvvkmezo.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gwrctmslq.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gmxhouhbt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gjiphweai.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gbkphzqpo.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/grbbkasco.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gnnngybvv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/geskpotco.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gkhnhunvy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gewjowaxi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gswzjbnmi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbvlhsok.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gcegkwjmk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gybqddboa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/ggjvmzzzs.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gmuyskibf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gofvvvjqh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/godricbww.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gwycbhlek.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gzncuqjdt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/guxpiziiu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gbrtqlalm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gclipjrhh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gubncfgna.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gyluoldjf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gxpiyvnzy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gscmogjvo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvblehbza.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gwpfrtkbo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gljgiefrc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gmcgfvbhx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gxnynfftn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gtitxyirl.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gaikmfmmk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/giuxqfokf.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gkindqpoi.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gparlhijh.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gxisfgmla.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gqnsgjofp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gbymslfyh.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gybuaifaf.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gxlzwenxz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gypssdxtg.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/glhothwvb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkbjifbjx.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/glyskdxew.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gyanyczwz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gmyksgflf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gfkogpjfb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/ghmadfkud.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gnugipgak.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gyjllrrxa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gsxjloons.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gvpeuohwe.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gfhmhrier.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gljpzrdux.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gujsstrix.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gqdckleuk.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gqgaccqkw.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gjiizvstc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gtctvvqhq.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gsyfdibgh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/grpfvmvbj.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gnmppffwn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gcdilmsnw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gfjzipsyq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gqkjxaiav.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gbcwoabug.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gpgqstjwy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gqvnzmneq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/ghotbpgrq.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gxjddeljg.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gpbxyzkrq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gbtlzwjts.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gibikymwc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gzcntmoge.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gurzyckbm.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gjkqpnkgr.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gnpbtlrcw.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gsaadousc.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/ghlmbxlds.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gbintghrl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gdnzusngc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/giuqdgwwv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gvodlmwek.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gmlgrpjtl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/ghrppojfm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gbjfpllol.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gstykydzb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/ggbupkscb.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gvvjujand.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gckbdhnnn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gnrmwpxzg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gcxuyhfuz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gzwxshjny.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ghgobgwnw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/grjlvertk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/glyidlcki.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gntylbrxt.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gealgphsd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gctwaibcg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gpnbvfvam.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gzrgadlak.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gzikxwzja.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/ghkuuoegl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gykhjjkky.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/giyjkzigq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gwycvbgbf.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/ginfdnpyg.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gbkzlujof.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gxpbemmmm.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/grnkskyyg.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gmcksmomq.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gbdgjkcsy.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gsnxuxwyb.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gajafoahv.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/ghrfwbdjz.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/guadxqxwm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/grwerfoea.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gbwiaackt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gzwozqskc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gloqgrazd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gtesslvgj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gjhzshpqi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gpmddovrc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gewaybzto.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gxqpzkcns.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gafyahgqf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gpydbpmpo.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/grczmtchg.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gvqdskhvb.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gfhabnaeg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/ganemcreg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gnupdmtze.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gcxiwclya.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gajaiedeh.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gfoenrcus.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gfsazrtss.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gamhwdijv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gqqwjcrvv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/ggiewqexr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gedvyatpr.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gsxlydqli.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gqifgpgfu.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gidqwshpd.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gruzgksfr.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/goxayqdwu.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gfkzvpqan.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/ggwrmvxlb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gshvjobuf.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gpenhhgpn.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gixllfzwk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gtpwelbzl.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gouwwjcoj.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gbzukkmwu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/grwasvfmk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gbsivbdkq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gverpjeog.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gsxpcplsm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gbuclrmcn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/ghvtcoybi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gshixvsfn.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gaertlcfq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gmbhgczfr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gqfffejjw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gmfchcqgd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gjoknyqld.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/guxfotmlx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gxufegsnq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gnklhnzqo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gamfrakxj.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gfdpuwowi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gbqdgjttb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gqsfbzsvl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsqycwswq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gosijefcc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gnmxnkzed.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxdghgelx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gydccofqz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gvxlznmnq.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gmgnwnerz.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gpvpsbvey.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/ghdsunevc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gfsiobszv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gopejyymy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gybpulzhz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gkeivtnde.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/ggvbnrtqd.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gmqbqjkhy.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gxwcapmnr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gejifvhmm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gcodwhjkb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/geiqjsfru.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gahxssdfv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gjwscleco.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gqwxarxwa.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gfflsnqzt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gvybrfbpc.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/govithdiv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gmooerxsl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/ghsqepydu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gzahamvxq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gurvyoifg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gzswmblwt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gszrtgtvg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gajcepdef.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gpnfgkrng.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gewspjrep.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gjeayhyve.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gpgrexswx.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gprjmynjh.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/geqctrytu.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gambilwhk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gqfonlati.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gpgtksqja.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gjvqfykfu.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gzahimicu.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/grzfjrjig.sHtML


<!-- 参考信息 -->