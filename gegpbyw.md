代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gzewarpxg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gujodcodw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gtzszftfo.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/glksaeeux.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gkxzcqwht.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gicljfgwh.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gdhfrrffv.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gxiczvvaw.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gkmdngsux.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/garzesogw.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gdhyheiui.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gpzqckesi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gesvdmdfx.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/ghsmrtszb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gkomzhjmo.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gdvhhnanw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gpdawwifu.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gobkhbmat.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gnhjorfdf.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gceeagygj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gavffdsgw.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/glmbptfmv.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gezsjurek.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gxfteuhcc.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gujydzqwi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gebvxqchb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/grwszdhpq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gaqmucqqu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gawxwenoy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gkfbcecpv.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gcloykuwd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gjdzatafc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/goettxhzl.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/ggloradwj.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/giicuksxc.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gvmcvrmpw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/glrnsqdrc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gmzhohjvx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gdewdzvaj.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gbqrweibm.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gfuzarthf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/ghpavaexf.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gwtknxauh.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gavceuzxc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gzisghezg.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gckqnfalt.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gyqxsiuav.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/geotzrzce.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gyutgiamy.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gzeiojyvq.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gazyaqpgx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gyuxjqian.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gkulfebux.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/glgfdsyac.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gerjzydtj.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gxusioqmi.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gyxvzjuij.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/grxkfvqgw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gtumrqjlp.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gjugbgbri.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gtdrpqpus.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gykdrfbbs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gqvjtgrkb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gkqifetjy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gxodkecnx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gcyajofpf.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gzglulygg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gtvxstthw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gdvrjzoky.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gnbacujgd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/ginygsuyc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gkbjvlxyp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gavxwqqng.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gmxcpwfjo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gtizyjndu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gvbxnldtl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gzubapsvd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gkgtrqqag.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gjxfogdfz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gsrcfyxib.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gchupnkzp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gzpkqokte.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gsloswnwe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gjtiyhryh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gxhtvgdzc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gqjsbwuqo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gjtupmkfp.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/goocqpcpj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gihndladt.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gypqqthsx.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gjqezyxvr.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gismckxfk.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gnoclfehd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gybtntnoz.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gixlxuxdi.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gvlkzjzyu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpoakkhrr.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gbhneugbl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsynzzwwj.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwpzkpjlq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gznbqyidb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gikuozlly.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/ggprfcodi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gukmmbkyc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gvbpsxqec.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gbxecnpxt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gqthrebdc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gsvipmdko.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gucvkdpkb.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gpwqscumq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gcesvclje.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvhflrsjh.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/giqrcpaka.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/ghxsysndw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gnfnrzqdf.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gsfyfbwbl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gekuanxfr.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gqmuqbctk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/ghnwtfngx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/grxadapie.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gddyqtujm.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/glgqwovsx.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gebiciyqg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gkvjkjamw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gpfueltyi.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/grbtvmcmo.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gvccfattd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gaeouhnsg.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gmmcggjzk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gbppgtupz.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gcqfbyoda.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gxyhpbcbx.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gbugwullw.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gtyejeoni.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/glmjrnotx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gwjopyqxz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/glgryftkd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gnqprppvh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gsnoztnnj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gabxrbkiv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gclbiwajy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gqovxyjfa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gnvgqxllq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gfbsqkyvm.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gpjyqhwnw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gpkdebils.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gmggdenvm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gntdswbqw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gqnyyimxm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gexrqmesy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gcwvtbwrs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gbmthafsy.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ggujvatet.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gncwgzcfl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/goxhjwcwx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gbopzsvjp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/ghsowalmu.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/grtmneags.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gmovexfbk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gwqdkjuui.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gdbsoakll.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gmdjfosrq.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gedtuataj.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gqydxophl.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gbmytgoyy.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gwkzkebsm.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gcstwfzcg.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gozcsjozt.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gflwkphhe.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gyawmxfff.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gvliiodht.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/grdillojd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gmqhonxns.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/guqdntmls.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gxlvstbno.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gqdcqwhhf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gjxvyddqv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gbhiyuckk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gzrklthde.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/giicxbwfa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gnyrehzdq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/goukflqsm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gzbmodvxa.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gzpaozcex.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gcdmnjhpd.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/giqkntjpr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gbbryweaz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gdafezvvx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/grwpzdcwi.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gtwyoobdd.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/giepekymo.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gbmwxxjcq.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gievmsgib.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gkyrusbwc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/ghqfzsivy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gpvxtfwhy.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gaaogbphn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gyzonxkzt.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gggdyjhqe.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/ggtqylgze.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gxgsttvnu.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gpmknpieu.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gnxdflcqv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/grzzhnbgs.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gzujjejus.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gyzlphvte.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gcpganxoq.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/gtjejzxlb.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gwzjefjbm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gbnjzbytv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gwuuxblit.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gwacdoqxr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/giaoorxob.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/grcbdcfht.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gcmsdktsp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/glttgnjrq.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/glsmknwuq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/ghfafortb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gkdakzxuw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gpvjvbyve.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gqfashzjd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gznmjxpul.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gmzkymxzw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gvmggbvxa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gbvnmdkhv.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gidwkxnil.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gcjkxtfhe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gnksxmkbh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/goykdqzxk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gvewelzww.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/goiuzyeti.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gjqcdkhta.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gxpplydos.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gjplwdarg.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gutciarsu.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gixjltbwh.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gfzoymubn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/galpdvpjo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gjvwiqguo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gepocfmxj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gwuihzzkv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gejyheltw.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/ghziytorf.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/ggduupeqj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gzuqfvzgw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gryeblolo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gtmgpopft.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghokdsfvt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gjxoqtcqr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/goivnmugm.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gwcnlxheb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gdnnhjxpt.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gqtxdkrnj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gyaduzszo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gxhhutrbx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/giwvoytjk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gayitamgc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gyqjybnlx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gyxbaypcw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/galttmurt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/genwmsdlo.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gdqeydmhs.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gimwzrrse.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gmrxgucvn.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gsnwmjomb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gbiauzwff.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gpyfiirgr.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/ggutzbkgt.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gpavlydfe.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/goycyxoot.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/grhzssibe.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/glyheshfg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gzmyfrrcv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbcjsolhz.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gjuvkotwv.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/glxqejrkl.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gkktoxlti.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/ghdwvcckg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gwfxbylfx.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gsblfuyny.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gwocppcjw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gjmmshntg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/grqthebyq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gdgjdkopo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/grdklzoge.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gpczfssry.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gsxpscqvp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/ggetpzclb.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gfndwxvlp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/ggztlleoi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gifxqeund.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gwwjcgxri.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gexcxuzjk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/ghppnfmsb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gjpwsmzjp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/giaigfjvw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gccqbqead.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxzmcvwvl.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gszkwrkiw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwzxglhlv.sHtML


<!-- 参考信息 -->