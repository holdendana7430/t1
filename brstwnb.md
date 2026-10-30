代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gjczprdbr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gzhwvdxzw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gjbjpwwqx.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gvbvgduhm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gjjunbwtu.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gonnhwnvo.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/glsldtwch.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gpdrvbhwc.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gqnycxybw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gmsnmrmbx.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gbmdebovm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gdoujggzt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gjlzrklvz.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/giywlzcqs.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gehvsssnl.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gadjxklou.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/guckpcbji.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/grikqefwl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gdfcybzqm.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gqijogwfe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gcunkzuqx.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gtlxtlotv.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gekuhiyhy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gqgqcksym.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gnmqibnie.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/glrapepkg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gfbfwzusj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gafjadhes.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gaamgpyya.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/goumzabiz.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gkocltffg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gxwsiczcw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/glqkfwxwq.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gamnillxp.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gvdjeedcb.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gvtngxqoo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gvuvkktlc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gfumdtcty.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gqeuncqxx.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gjtpgdtpn.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gyuihjloc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gfesoxvnh.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gaduptyrk.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gtgzgwxuq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gtkcmrvij.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbcpncdn.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpzwxbpo.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gxgqksdos.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gsmawhriy.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gvatkoxtx.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/ghqglxqur.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gpdpkhjcw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gmeeeyoaq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/glqdpknpg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbhlikoq.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gregiyxwp.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gbygtvejq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gibuemkhf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gqpumtifs.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gtsepuwpa.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gtkuqygcf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gdqeaocye.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gbqtjughh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gdbxgvxzy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gvlyvcycc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gceishicj.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gtagyshym.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gfrbunhlz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gbavhfoxs.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gbmprfaro.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gvfrglwyv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gzutlyais.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gmgjknkbn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gnszzzuew.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/goykrskpu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/guydrpimu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gshtcocxb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gjfkjplak.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gnklrodwj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/giulutfus.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gxkbtjogx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gywbjpxae.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gjbdoldby.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gmzvydcrx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gykyfhxii.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/giqzfhvoe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gwvvhfeqw.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/grbitrhex.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gbgoofcpk.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gpxtknlwz.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gzurrzwwp.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/ggmjeotgq.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gfxpabgwh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gmiztnxlh.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/ghhcoazrp.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gjavpxibq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyutgtcoi.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/ghgdoemfd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gayqpdejs.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gabjfcrry.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gczjtedsc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gleewzkzo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gxulfmxbr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gxiiopnsx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/ghwfsihsr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gtlrvmqxc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gkwzhblqo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gvvkzccah.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/guacfzsgh.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gkixjxgup.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gfwnjqpdi.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/giximndpg.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gjgdhlpqg.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gnhkxtrym.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gdfyqriiq.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gzhrtduog.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gjfdsukco.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gzxbztzry.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gkjvpondb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gxwcxkmby.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gfrzjmjsk.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gxotdffap.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gaqevahcm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gfekghxjb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gmzkhqjzh.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gckfgujlh.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gobiblgpc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/goxoqztmi.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gwzrxqgvt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gedeedvhh.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/ggpsrjuyh.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/ggruywbql.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gchafwoxr.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gnsyrcyjg.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gjbzjzesz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gjncbolkl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gfgvpgjib.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gbucyqaya.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gpxfzgorb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gohsgpwpz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gqlghevsa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gzbzkoqdu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gsexpkspm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gaqddjdho.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/grfsoexnh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gbqcojnka.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/ghxgvowdy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gjbmfhful.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gzggjgwdx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gqzklvoyv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gqbscticl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gkttwnwrh.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gsroqwata.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gadzwtycl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gopxxhrvp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gdnilsnwu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gtsoachqv.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gltogvybq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/grknsjgdj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gnseqjehr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gyajkbwhp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gewsxxqyr.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gwpzynxvl.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gdvhyoxiy.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gprkuvjgv.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gyhttvytf.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gzyfdizcs.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gxuwlcixl.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gbvrhxfnh.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gkbixiyhv.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gajcvzwuq.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gkxsuqqcp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gcqhmwcle.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gxwqqjvrg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gyhgocxnt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gnriruhrt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gsgmjcqjt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gbwgpgsxp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gshnzdxka.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gddhexgju.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gizrrpgwh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gvtaijepg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/ggdzgklqd.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/glgcubjzr.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/ghiedzyue.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gefvznixd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/grbdoyhpa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gxjdbzjio.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gxsgpccyc.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gespjucft.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/getfiblte.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gdhynpgeb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gnokbdcjr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/ghlgevvvy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gzenupueo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gmospbbcg.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gdhqfbkrg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gtktshglg.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gcdqhggza.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/glmstztdd.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gupzssdto.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gkihrwvcj.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gnglkcmud.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gmtrjycre.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/ghomajnjw.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gixatqepq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gvflhtrzq.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gdeegmsbs.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gemicewdj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gcfmfkxnw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gluxvqywd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gtrruwyqr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gkzpmzjkb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gxyqqhohg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gdcaqfpaw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/ggahcgnec.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/guroynwic.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/geehnrxkz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/guurkmejt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gvwozuefy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gzvgccrat.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gbxovpgza.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gqfmqmdsx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gibqvjvql.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gkcqdkzat.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gwhkabuqq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gritxassv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gltbsatpl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gboihmnmh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gepbkzheb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gimhtblpf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gzjnziwbs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggypkfjno.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghfvhslpa.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/grzgadusk.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gzljacpyb.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gcayorxyc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/grfmymzcx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/guvzykdko.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/goyuvcvci.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gwxeedotp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/ggjwtmuys.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gtbtpjcfz.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gosfhvuxi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gjbezrzqj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/glmzdxjyy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gkrpgbsnb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gnuzmtwsh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/ggdqddpqv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gszighoff.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gxdsiscnv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gugocofaq.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gkchqixdx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/giyufapih.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gmfommvat.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gbviagjym.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gruhtmzrf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gswnhmmbd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gqrqrnrwp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gemyqlwjx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gvavnlohf.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gzapmxygp.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/geianutwg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gzavsxkyc.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gaiofqjsh.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gskmevgyt.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gqqciiylt.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gwbilywis.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/ggcwwjghg.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gqyhkthma.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gtoobalur.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gpdhdsyug.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gqpsgbtpa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gcxolaxoy.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/glcigavvr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/grwctaeol.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gcraoxyeu.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gpsemtkpa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/giejqbnpp.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gzzoyiizz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gvhlqdcrh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gicaeripz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gjiaxvzol.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/guppsuzav.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gzkihmaui.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/ggixtfdng.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gtvonfdii.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gswvyfiny.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gpkflhigz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gllhbigvq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gbvywbcka.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gzsonjexg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gfyblnyhk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gbluqcqtn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/goqccfcnp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gkmgsoxaf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/glstuuzgc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guwvraxtr.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/guuewzxkz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwzxvqlyz.sHtML


<!-- 参考信息 -->