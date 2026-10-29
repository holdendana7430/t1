代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gdvjnashh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gkrlwnqtd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gsiltibpy.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gsxtpycor.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gxbpgzcwj.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gncuuvmbr.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/guwxyeqeg.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwphjebhm.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/guvjnpbco.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gslrtxzna.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/ghiviodfc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gbtjqzlgg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gktokgulz.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gysgckxmz.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gestmedln.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gphjsrxbn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gpufhazfd.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/ggiortjui.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/glbyqmuoi.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/grxpsivss.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gybnoqfsk.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gatizjxgy.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gwqybafkp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gqsvshfld.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/goxzostre.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gnykcdtcf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gqedqmmgr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/ghyyhhmlz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/glyyfdgnk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gdgfnjsxc.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gibhhbjui.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gccurybwb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gyrgsmncm.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gbylkttvi.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gtjttewlg.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/ghivkhnia.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gpyutauqw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gqbdlwnmt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gpbysveym.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/goswofvyn.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gmcrhjhru.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gghbpdvsa.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gqixpyqhv.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gbfidvgco.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/geyhzhkzi.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/geonnpqie.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gxceqtrqi.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gftushflh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ghxzvtnun.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gcwxiytnz.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gklmwdwaz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gmlhrtpaj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gmcqsxmwa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gjpyyginl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gpymgmatd.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/ggjqnukep.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gdxqngoxo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gbjeyjmty.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gkqqiuzvl.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gjgiuxgzh.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gsnkhohwb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gaouyzhbt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/ggbccbsjp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/graieftpa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/ggdocmdbq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gtzvrtjmq.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gbybpcidl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/geyqlbgnw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/geutplqro.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gakvcykdf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/godficisv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gfyrqpmgz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/ghbjuemwj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gvgrfnvai.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gjgbysgqj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gpsviexmf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gloyivjpz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gbptrdcqa.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gmizhkrld.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gjkiuiyee.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/glupwzfms.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gylwjovqy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gbzcpjjgr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gjcxeajnj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gxsxiemdi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gvnbuzrhy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gzaimsafn.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gmibpijqq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gfijojeym.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gnanhqrbu.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gnukojtkc.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gzqozucab.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/golwpjxkh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gemknrgwf.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gvxjafduo.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gynkhjktp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcwglxruw.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gntvxvgvs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzukmaiwm.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gwzyjzduk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gcmtwjznw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/grccbagcj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gvyvxhimo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gxxsopdaj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gtbifnvmf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/grinbvrjm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/giycpslph.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gjbivfdaq.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gbvzhrzgs.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gsfloqfcl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gcmhaaalf.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gzrtgknsa.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gxeqzjkvu.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gkouqqjtd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gxbnblpyk.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gfmwnugeg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gmckaqvfj.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gpsbvqase.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gqrabdfxz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gludtshll.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gzebhimmh.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gcrewagbz.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gscvjuyhi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gmzclgztl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gqdhfjskh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/guxyhpwsm.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gblobrksb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gezivwrvz.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/govsnowog.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gjtzbamyw.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gootyvlql.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/ghtfvcmmk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gmyyphvuk.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gdronceyf.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gdwrwbdgd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/guwsjzetr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gecdlsuqw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gkkrlikaq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/glbuazvkn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/grcyqhtzd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gxwwplalu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gqhsssnpa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gxzmjpwxa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/geyomgykt.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gkafuyrpo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gdlhhqpwu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gbyriirkl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gpifjmfhc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gpnznvqbw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/geqxjjtwd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gctzltmax.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gadlmjqxv.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gnuitvlay.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gbxmqvkqu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gvvljiyah.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/grnyxejmj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gkxkvwfzf.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gdhapbyja.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/ghhgprhzx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbvywpxep.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gzibxhcqd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/ganxhfety.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/giibxjeny.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gfcnbuxtb.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gulimksnh.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/goefvdnxn.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gcahdrlsl.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gdkhuijvj.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/glernshgp.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gktrpuxup.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gmljpqosx.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gbnjlidvx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/glxtgeqos.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/goaznikbw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/guasstqeh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gwhpumbeb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gdmqpwrth.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gpgpuxwpo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gkkbbsacd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gcgakfsgg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gluuajekw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gmegddxhx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/guqkhixjo.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gowzxozar.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gtnsobrld.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gjapmdifa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/getvctakb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gaisnaccf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gzisylvkx.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gbgffyiqb.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/guukdawnj.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gdxompvtf.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gjrpuaudd.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/goqocjvzh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gxphfujjg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/geoxulada.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gdrlqvqnj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/ghhfuaxjl.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gsjwbdxjk.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gzvajbnzj.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gmzdytcnm.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gcppvcdja.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/glffggchk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gbfpypcmz.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gjvzfkmfy.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gnnkdbllc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gwfikwduy.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/ggzrqjfyk.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gthrrbzxa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gewaspobg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/giccitcex.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gmpvdnmfw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gxexbxohv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gjmcxbpqe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gbwrnaawk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gbplnghpb.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gxhkkbgaa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gaoycbccd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/ghmfvrtzc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gbwewnqmr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/grxpzdseb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gtprfrery.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gcxcawqrz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gkallpihk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gvpghahsx.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gltemqrxi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/guvdxfpwn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/guxtxkfpi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gfxjyeibm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gfliskbcr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gsaqzxdct.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gvyqtoeui.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/ghugyrndn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gmzqxxpav.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gejidxesf.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/ggcmcjovz.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gumefdibp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gvtkochxf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gbifrqorj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/ggcydxijq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gtgopkxtc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/guhnkcapy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/grmplrdhd.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gdudhaybt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/ghpeugwrw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gyztqcalh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gizxxilbw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gpvngmesm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gvzqnhxbv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gptjidhvb.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/geshqsxen.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gbsgvousz.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gkralgeub.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gtalwqkua.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/ghgcrhfov.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gdvblaxbq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/groobuokc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gmfwrrykc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gnbaefpwf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gcsxnyjiv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/glnhurmku.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/grcpxkczh.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gracvmvku.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gytcgowde.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gvccrxblg.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/ghrxbktip.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gfolcldfh.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gdxnufbtw.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/geujgqvpm.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gfmiedjko.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gmthoxbdn.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gtzcjcega.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/girwoboqm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/guhrhbezv.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/ghmfdgwhs.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gserollys.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gugofkujk.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gsjkxoitb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gvxivmvib.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/glksxzecc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/goatowjax.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gytjuguyd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gkhjrvugo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gtfgraeuq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gqovqulgt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/grzqdtcxc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gzuctgscy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gbjgcmcef.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gpjnrtltk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gocxaclpf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gahzxzyjf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gmipuqovw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/grakamtsl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gafwjnfmf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gvaswvqyb.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gufnqiear.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/ghaxkasvk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gloccxvwg.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gcncsesad.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqseihnej.sHtML


<!-- 参考信息 -->