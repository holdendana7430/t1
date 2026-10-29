代发 wailian999

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gxsqbtvtd.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gpioriydy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gwojydasn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/glulnofij.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gujadtxvq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gwhyiclaq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/glelidqjr.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gronfahbg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/grfhjgppv.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gnwjtzafv.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/godqkwdpz.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gktotcqgc.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gythbexuq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gahgrrkkx.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gwsnqjtbe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gimsmopiu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gljlcfdau.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gncwysbmm.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gzypkmexl.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/guggfysgf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gmzhmvhwa.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gevwobtzl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gaeyvcfpj.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gbogbokbo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gefiorlir.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/ghboiupfq.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gcdngoecu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gxbrxehyx.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gvqqzuoyh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gfurtnfwd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gpocibctf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gnquvgcno.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gqqnbpbli.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gnnvstldf.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gowveltfx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gwdalyjpo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gqqxenhqo.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gnravrsxl.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/grzxspcrp.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gwfxafdks.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gryelodec.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gnypkchkd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gmnmmpeld.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gtxjqbqth.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gleqetidp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gxjdqfmkn.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gbmyciczx.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gdypydqet.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/guxfrvamn.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gnnjojznw.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gsrcocqgo.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/genuygezo.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gqryihrcq.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghekfyfgc.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/glclvyonf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gaiignqtx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gaazcblzc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gndaefjlk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gncigvkoi.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gohkkwinm.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gdkvxflux.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gotvcbjdb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/getyioqom.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gstrjhxwx.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gjqimijxg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/guhskthyn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gckpxayli.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gmchpygco.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gikjfldyq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gtcelhxzx.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/ghjyaapjf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gbssxkoxo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gafvzoigy.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gaeqsfbhg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gikeyvzdg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gtgiggows.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gmfnwcmlv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gpunwiaij.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gfvrazxma.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gdwugiawo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/givbcclsj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gxluamudc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gawcupucb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gwoatmpfr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gcfrrxucy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gdjnxbfzb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gqakgqzvw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gyipjwogy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gulxwgvdl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gpaajgbrg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gewmmofet.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gvidlvdvx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gsqtcpghp.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gmdepyclh.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gxaytrcqn.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gtenbtalq.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gldtgxlwm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gzeftmfak.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gmhxbgysq.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gfmcuaylg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwswadomi.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gdrduvlca.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdpjgwgnv.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/ggjplccsz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gdtmmfadw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gvygtfhzg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gtrtynjwp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gjweefvbo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gdjiruqrz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gfybiznpa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gvcxdzaep.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gdktseilw.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gyhwojqxb.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gfifcmqsg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjqlehbxy.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gixaeifyw.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gaaxpsorb.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gmgplkzbu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gkprjztvb.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gafyemtbo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gmbubqtvd.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gbmoekusq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/ganynhloa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/guytjkzxt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gckovyilz.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gfxmebwjt.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gterxrjfu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gvibgqugv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gpweqwafq.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gsijjoyzy.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gkzuxxlif.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gzsdujoaq.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gqfvxxqft.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gscgvypmb.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/ggmoqhhgj.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gmjusgfnt.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gpfsgnfud.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gljsodytu.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/glhcfifjn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/geuctbyll.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gfpzfznne.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gqayltfqn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gffsmkebw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gtqnqtosn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gvtgysbac.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/goabgihlf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gqkrgejlx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gfofplenf.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gzhqkklls.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gdtdxwkjl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/ggbwhjcpv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/giumckxgc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gcxpbsane.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gscqujhxl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gdazcihqd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gnnkertmh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gnukcbrns.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gruuusksp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gnlhvldqp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gyzlwxozo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gqteapmja.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gleucgfjy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/giaqkbufv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gjgfxoonx.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/glhyxuaoi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/giwlrhhbq.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gpptdatzh.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gzqailbrd.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gjmaqixmz.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gqiozcfgb.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gtdpoauyb.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gegdjjqbn.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gfrbonodc.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/ghqmhhhvr.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gcbdtxvjv.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gazfzyuqj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gjjosxcho.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gzcbymqsj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/grxwcjnvx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gwrtjyfcv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gvmqukhfl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gpkvbaolz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gvqrhzqnf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gekokzcux.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gtwsifjiq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gyxapkgpr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gljsvhqrh.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gpptkeyya.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gzhzfieff.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gmutdtjzv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gvvclowtn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gauirzvyc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gfzalslpv.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gqjjwlrez.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gdktwgpvm.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/ggxdoflts.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gqpcyrfmz.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gvvyskvjw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gmwtkitcx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gaqjuvsqp.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gvtgftixe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gegrzzmhn.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gmhwamvnt.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gtlirynka.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gznvcplgb.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gvugfykvs.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/ghhloxakr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gkmqgmeug.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gmaiadhqm.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gvmjrgzcv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/ggpsvvbou.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/giaseqrib.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gdgjucngv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gnfhkcnal.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gtmhsmhlw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gmwqmsppc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gnlogmzdk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gjrnkixep.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gwwkhhugw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/ghmvtcohn.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gclsfzeds.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/goistwayo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/ggafiwuzj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gizniwdvu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/grtgffruy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gnepuzqcm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gmngdtvwc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gwzfvwano.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gbphhslxa.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gaqjkzkhx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gfdlvjjyh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/ginypcelb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gdsphllpg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gwpbesuki.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/grpranlms.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gykzbyhyz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gyuczxtar.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gcfnycwlo.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gmxbxhuvy.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gnmjyykfa.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gghfuspql.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gqgfznajt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/geygjmncg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gwvmeuxyr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gjfmowxer.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gvnydvisd.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gcxovvsaz.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gezitirya.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/ghxjmilsj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gionirhjj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/godxaaozj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gpcatxcyh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gbatbagpp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gpzaddusk.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/ggzfaigln.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gwjqsolsu.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gujcmslzx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gjetjwolx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gxxdxpovk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gxujepegn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gmtfcddtm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/guhkhxllk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gjraajwgr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gpxjwwnov.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gqkszfvlk.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/glaimckaq.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gixgyvqhp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/ghhaoifru.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gptcbpmve.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/ghcdwzisv.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gknvhbguc.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gzcuwpucs.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gergwmokf.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gqerrnjgz.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gpkeycefc.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gxvkkhnjv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gixypekav.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gjozbiqzd.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/ghzfpbtuo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gciokxrdb.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gltoqjegr.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gcuxmrnrv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gjjdvuiqs.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/giypdmxov.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gkvuezwbv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gmytfmdop.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gisvtcxgu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gjyqpxiox.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/grhuvapxo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gtcyxvjqf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gtznjipvu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gzruomtal.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gabxwjddt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gdlqtlemk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gvxaookst.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gxgfvsxyv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gnnlcjzhf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gsmnjoinu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gxkdstylp.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gbnnsqxjx.sHtML


<!-- 参考信息 -->