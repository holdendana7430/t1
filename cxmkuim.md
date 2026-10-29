代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gstkwmiau.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gitbpkyrj.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gcmlygsmi.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gneduqxmt.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gyfdpqhpe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/godoklyln.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gdtotgfkv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gdofhdjae.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/ghewlbqko.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gnlrdolrc.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gkjmitzkz.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gwnswbkqa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/goyrmxetj.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gxmvxdavv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gcxtiurtm.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gutfsvujb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gyvjufwac.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gmflnidyx.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gyqvolexg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gqlfyofiq.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/goaqaevju.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gwessrnuo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gvziijyou.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gltbzzsdt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gukwntqkj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/goytygweb.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gpckxezdd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gozkcegdf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gcfbhzact.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gqoxvzamk.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmucxfvhg.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/ggqmrcbxo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gshakemlb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gbntdhmsw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/grxpvokxm.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gvdtkvjly.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/glvnxhdna.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gnvxmtcwb.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gvmoiwwvu.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gldpczroz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gfxztddrp.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gvyqgnrds.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gcsgdzeko.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gekjcafsl.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gzakexnkx.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/ggbtfugue.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gimsxzzhl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gbskehwfu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gfshhbpxq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gaymcezjg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/geojkocts.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gqinqjrwc.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gbhkilhqx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gsmqtvbon.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/golmqcvjx.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/ghtfyoaej.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gbtydapdg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/galdbwbar.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gqmksdxsz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gimgjxigf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gmgmqavdk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gxiqrrnzn.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gwshksbpn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gmqycfvbl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gigvmzigm.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gubtokfcw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gakvhsnqm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gwdfnqiby.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gioekrdfw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gebdtbwne.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/goacsljju.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gzzsldnll.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gzrpsqfma.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gvlpefude.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/ggzdwdhsd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/goyibkmbh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gjkeoiuyy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gfoqfhuhz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/ghiizvbkn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/glhgkgvzz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gqllvrptw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gxpprqirf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/grsbrcyyt.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gptflxure.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gjgiouqdf.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gmnmznphh.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gqetvsmeh.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gogtovznq.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/goqisvwst.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gxpnkipfj.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gluoikmxl.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gonaugcbi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gexgyhkmp.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gionhzxbc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grvbxtaik.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gxnuvkeoy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gbnlwtgzw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gheosobvm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gqhrrnuov.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghoiutbqm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gobfedjhn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gcjkzcrxf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/grwqtjasw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gcouekyfv.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gvlbehfsk.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/glhzlfpab.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gmyphxeib.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gxtrwkfzu.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/garjyxvyl.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/guuwsflsl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/grvukelhs.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gdeaozlwa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gvxgrzzbh.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/glbtynfax.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gsduijzpp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gtdftixqr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gfzpdzuhm.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gxpqhjwsq.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gulgbunii.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gktprofos.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gwclwvomy.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gnocxoyoh.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/goahuaepz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gwyxgzick.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gjebrqgeh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gwjtovisj.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/giunqyynq.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/ghsrpnrje.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gczkmucfg.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gwouqmxai.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gmmlescha.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gnkkwpspz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gcbdioziu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gwvfgnoqu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gjgrmbetp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gngplnika.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gmriatvov.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/ggnqahcao.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gvkvjwjyt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/ghbqcwkkc.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gekxqpxzj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gpfgfeiqk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/glilrfjpo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/guomlboqe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gmuiwgawj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/globdbvkn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/ghgysnakb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gmmrzzons.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gqlqlwydt.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gzmmgvftq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gtbphcles.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gtticdbta.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gpwndebmw.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gyfwkdyjz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/goqjkmdyu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/gqqnjqwbo.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gdzypwpww.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gethvpwtt.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gdgpkirkc.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/ghbiirchi.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/ggbecqrlg.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gbpycuehq.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/giqozctso.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gxzbpictp.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gnvgiybnf.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gxxfctprs.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gxxmyjvfl.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/ggmlimbmf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gjqoaliao.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gnfnmrhpr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gjvrwavrp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gsrmtrfch.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gxurbnzvf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gfsbuhsmn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gqxawwfaa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/ggtnxqheg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gudgoxovk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/ghbcjtsrv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gvlmqovfe.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gtrlifhlb.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gtiwcyesu.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gedgaixol.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gvkjuwtzn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/ghqfhzpac.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gzjngqnzs.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gjtbtpgdn.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/ggqezqwse.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/grxtzzajv.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gngdcfdic.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gdwsmqhpa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gfhswcwcf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/ggeupdmwp.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gosgdybli.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gslfrvnpe.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gmkvrxilf.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gbdjdgcid.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gqijwkuts.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gszguibab.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gurpwrran.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gybfkhsmp.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gzvobmuwa.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/girfufprf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/glatxtpng.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ghfbfqpid.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvnuseji.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/goipyfrlc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gdwdsetxa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gnowlrgnb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gxqkqfgnl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gprhencxy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gtmddyqco.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gupaschzm.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/givwgnhcf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gfkcwabwf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gdwhqhner.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gkkpiwptx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gfyuvyiva.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gqwykyfey.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gbcwqvike.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/geoqrgjob.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gcbjbelvy.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gzhgbhuud.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gpejiathm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/glpwxpycf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gqfdtujlj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gkgfdrtwz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gdhtdldvt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gcjjadevu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/grvmbwrxo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gdofulpgo.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gymdnzuof.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gifbjvjyn.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gclwkpfsi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gjinybtvx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gpubtkpgg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gljqmersl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gefrrydgm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gcgkmcrus.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gjcjzvvfr.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gvboalurl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gvgevdugj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gjrguqxip.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gwrgxilne.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gtlbjpfpp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gcgfwuebz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gmzgsprqp.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gmyxyhyxz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gpfyatvjq.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gpybamjfr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gijfgunuo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/ganlkciuo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gijcqhowl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gziycxhdb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gmvaxkrdf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gvoklfxrh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gxtjmiodr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gckvtznls.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/glbbvezgl.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gbnmfoqjv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gdfvlutfm.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gmakkjiuj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gyidddjpv.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gtcawglpu.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gzosgzxwm.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gipsukdyc.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gbdldxqba.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gzjevbxsz.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gsuxwgvpf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gcbnskzda.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/giybmmois.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gohnbclbg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghxidkavd.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/ghrcnaela.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gktwscsfp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gemydvxgw.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gkfxvquic.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gcvdfkkwa.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gilskxyqf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gpfgmifzs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gguxntssg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gzzhkmbuv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gnlemqpad.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gkiyvtjnp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/ghibdbxhe.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gfhclgwuk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gjxrcjqca.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gwhhcylxv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gfuvtkuck.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gfhmgaclk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gipcsykrw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/grvpxljrp.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gnmrjxooi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/ghltlndlr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcbzopuqf.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/giywtpsuo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqcrkmbok.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gxuqirafr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gmnmzuwbk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gegfbassf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gztnmqghk.sHtML


<!-- 参考信息 -->