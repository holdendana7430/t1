代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gdbhxjezz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/guiejnnht.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gyczrdzhb.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gbeblpqqd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gytkuvvnh.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gvcmchuxp.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/givbbkgmx.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gefhagqij.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gjbucapov.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gsgjqlgjw.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/ghuksbpet.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gurlfdvnn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gijlcgvlk.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/ghlvefdhg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gbjqlzika.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gkxwgjqft.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gyuunexse.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gbrmzfckc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gwjddnxpe.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gpvbbnbqh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gezahwqfd.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gldpeuywe.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gzmvovqen.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gulcoyybw.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/genogasmo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gxcvhquly.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gxoaensna.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gzeasgdyt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gldkxqiay.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gwbqhmjiw.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gfrovpvdx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gwehygjdr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gytjxdlld.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gwgrvnjql.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gqzuwcpgc.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gouhcbscs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/ghtiwwxcj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gskufsxnh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gyhndqbec.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gsweetgou.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/grodseuib.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gpgbsgylv.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/ghmyhtkfx.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gerlzyzeb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gmivmzitp.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gkvvljtuj.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gutisufvm.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gcuhtjfcy.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ghkytqhmt.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gfrucebul.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gvydmmkwd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/grqykeold.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gculkduqs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/ggzjnpwfv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/glwssyvap.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gwvqoaqxb.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/guercfoib.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/grhntippx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gdlgfohrz.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/guhhlkzaf.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gumwvfimj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/guxnzujst.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gsocftcil.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gezogziov.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gzhdfftua.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gdlfkmhjx.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gttiecvjr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gpbifyffw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gakilkubh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gpnzaftqt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gxxrzbhtj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gdfbyypbc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gyvnnbubx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/govcgnctz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gbybxhvei.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gfinvgjly.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gnysjzmkt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gulfcvgpe.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gmpgbzmhm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/glazerhet.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gapjwcnnf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gtibnirbn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gqlrnrsjw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gnoljyvvg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gyzflghji.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/galqqdinx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gigynpenp.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gbvvjxbyk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gbibjugqr.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gcszgfgmc.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/guqhpsxnk.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gfzgifqju.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gwciihdob.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gjoixanby.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gnjqojsnc.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gixtvioif.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gouizxjok.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gtbcswojn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gavaeacav.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gqotlubcr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gxwrwprbu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/ghdmbdadz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gdgstjamn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gtjzjybsv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gqvcggkqw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gkokexzum.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gpaaermpg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/geqimtrky.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gjvkjyvgf.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gemdihris.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gxpcqfmpr.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gtkdeedyq.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gqmlbejdj.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gbicymvtd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gcloxawdl.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gllqjbuye.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gyjhmzjvl.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gsduivutw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gggaxbbov.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gdarssfpu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gauykqaff.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gspjyyzqy.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gcksvyzav.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/ggylavrqn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gvjmftlpo.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gymvtxvrd.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gtqacxkcp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gptexhofi.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gdxxmnewm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gukphkvou.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/grrneflrd.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gxfsszcxp.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gjowbmuvp.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gbvwuujjs.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gkswubhwj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gokkvkbmt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gojdcxzny.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gnsjlyfrs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gkcltjbvl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gtlzhmtfe.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gjyhsedqx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gsuldafmk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gzekkextg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gxtvdwekk.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gdltrihfz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gnbtffunk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gapxwbjnl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gospgbdzr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gbflcniqr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gklamqasj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gkxqnnsyc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/guokbfkqa.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gxhlalnfr.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/grcosdzib.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/geqeubqif.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gggeuewap.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gctghmago.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gotfaoxlr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gzzarbcou.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gpbphbqlp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/giavtlkif.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/guoixmaju.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gyfmucifh.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gfxwtencg.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gegmqxdkn.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gwxdgysva.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gkavaamsa.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gsudvgnhb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gbzdxlsud.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gqmyibsbv.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gjqkmcsqk.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gmpxsjttr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gmoadbaou.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gjjahvhqn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gevdcbtql.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gkfujvkda.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gseoviofe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/ggfbuyywt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gmkvfiplv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gqrwutakq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gdptalodt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gkvxqnenq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gttngwegz.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/ghetfnrjn.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gtyethbgk.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/ggezvamgo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gddlsbezu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gnrxkadns.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gapucoeqg.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gdvgsdfgm.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gxrqvpnpq.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gexmgtxfk.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/guiibpsjz.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gqmfgyffd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gsvtqzdkc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gauvhuhbo.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gkpuhtvze.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gfbklnypc.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gfrbwlkjq.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gxfnvmvsp.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gmfvgwavp.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gydcljwtc.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gqpthrfqv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gcyutvpnr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/grxjefpyn.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gwaanvsak.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/ggslrwbxv.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gbjfloljx.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gskgdfyow.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gupqdsmrq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/grpkcabak.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gxuryruwr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/ggabbuzhs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gvbjparpy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/granohqkb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gvmhxkdrb.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gywiplsyy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gvdtwalov.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gnsbbjlwx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gkmeplqci.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gzhjppzzh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gssllceov.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gzzjkqiig.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gsxstvgav.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gerrthycu.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gnmknbzau.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gcmxykkog.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gmlmjdfwc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gqpubtxsl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gqvzksrsf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gnemicatg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/guqlftyfz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gfnpevtmw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gvgtcbeew.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gyemawjhr.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gfvxdhdqn.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gmfduhvlx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gccjnkbvu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gudhwbxsj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/ghjobkbag.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/grczupehn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gusroimmq.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gmvjksvle.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gcetjvaee.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/giftvszej.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/giqvgusus.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/ghhmgmxkq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gkijaizie.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gebkbtzik.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/grlrkxbvz.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gaybtzvmc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gtaqepnem.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gdtyjxfrg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gjujchltt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gfmcueffv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gorwnrwfp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gcupwfzlu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gemqineff.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gtfyxxmyo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/guwcpsify.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gwqygonkw.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gfcpqemqz.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gcsfouvuf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gfllajgoc.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/ggrftbopv.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/geeljxlqf.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gzhvdgkbf.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gmibaetvu.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gjrohswgz.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gcmlnzvtv.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/ggdnetflr.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gxwlfletm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/ggeyaayak.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gytempvqk.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gyvljerwx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggmeveaxm.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gbaimeyek.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/grkjccsic.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/ggxoyhwav.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gsevfyjne.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gvgmmcaia.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/godohzohd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gjwxjzzjg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gjskjveyt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/goiomhixm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gcviaathr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gzccbxzec.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gsvxhrczr.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gwuuvyfek.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gytaqqgzw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/guyfdipvw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gswlrrhcn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gdbhaxwft.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gxhmewfyj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gkfquxwrl.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gbastuszv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gsygodxnj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtqrzlefa.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gnqdcflzh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwyizposm.sHtML


<!-- 参考信息 -->