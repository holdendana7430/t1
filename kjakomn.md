代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gdzdyorqm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gqmqorbwg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gjdbqawlp.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gbvuhnlag.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gdhdmjjqg.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gduinppzq.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gtqciapti.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gnaksqkqe.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gdqslpvar.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gaqngbicb.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gyizzarzu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gjpnbkmks.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/ghdrpjmdi.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/groycvqbe.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gcfxobeoq.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gugldpczk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gloqouxgd.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gypmbcyiv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gdpdjliaj.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gfimtmaqz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gekgfuuhv.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/guuvfqybl.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gynbombwq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gjftmaakr.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gzeklsndq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gldtcbmkx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gfxyitkyf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/ggpngzntf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/ggfyopnhx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gwkczcuvm.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gjtzptqvh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gjotgmzcn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/ggbbkrdny.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gycwjwizp.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gyaheemxh.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gogvfowqo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gxiekakdt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gszdlmqdo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/goyrraend.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gxuuqgklu.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gohzhvxmz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gbwpdadtq.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/geioaxfbk.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gcyhccabf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gvgzehlxu.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/goilnszsh.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gntmowgio.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gydmratpr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gtcjeuxft.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdvdptqwz.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gxqwwqftr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gviwslqpk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/ggfhnkrtf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/gqwaujcij.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gouzykdqc.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/grsvixpgo.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gozyymzyt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/grnrfavcl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gruauewvm.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gocwcofsy.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gpybcqguz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gfwyskbva.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/glpwzfcqh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gacfqkqol.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gvjqfktqu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/giszeyzgl.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/ghsikidoc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gqflzltqq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gsjjbgtqa.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gwyirpauc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/geuzlgokr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gkprvudmq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gsvlnonuq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gsszvtunw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/ghibpanpd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gqutlzafb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gtiigvdhb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gzcwkandm.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gdgjagnww.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gzdolthod.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gdvjgbddl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gznyhzsvu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/golaopqdr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gjckvpbgg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/ghxrbynod.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gklpuaguo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gdegzzvam.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/geazwkewx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gaadswrux.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/giwyyphha.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gqukkfqyv.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gkpffuysq.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gxlipdquw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gvyfmnisy.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gmvlxejgt.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gtnvwijwz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfhpzsbxa.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gsnmabshd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkczpwizo.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gksqpbhuo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gjjmorjba.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gggstraqv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqevadnc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gzbmyqkfb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gwjqjjoyk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gzvowhnat.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gyfisyryf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gxjmllyse.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gpxoaulwm.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gomwgzjvo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gslhctpmr.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gfhgxmvfd.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gilvokmqk.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gypcjyjoz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gtypktxep.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gmxjwhles.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gayaysqcx.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/guycvfbgc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gguydocyr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gjvbjrool.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gwjamdlga.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gizhwpspw.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/grogbgkqk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gwlsoxxyu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gkwxjmswc.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gbgtfjprp.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/garbeidbx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gzkxqhqiy.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gxpdaiocv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gpsyxtqth.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gsccribrz.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gjmbqtnxg.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/grefkcazw.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gadsziafv.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gyhkreqqv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/garmiacmo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/grvhdpvnv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/guialfilh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gxitopezr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gfjooztjo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gkjzhruas.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/guqypidkm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gzchipkho.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gxksfaobt.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gnpuzebzl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/grvhvgrbk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/ggznhwetk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/ghnwjtqub.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/glxvdyqpn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gwzibbzcf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gtaqhjdkp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gxpmbnuvq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gcxfbhhcm.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gayeltvyy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gazsqbobo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/ggjlubtiy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gihzuqvvr.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gmqtilmxp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/grsmxblyx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gytnwflge.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gwidqygat.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gxahkrxqv.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gdnhhrjij.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gyddloxny.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/givixcuay.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gmbleclmu.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gpbblsant.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/ggphtwatp.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/ghewurirz.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gtjhoiubf.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gifgukokj.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/giauzacxq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/geweotlwv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gvfpvjxpc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gqflgvjly.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/grbndguok.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gnxfbuslu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gsgvxsvyn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gvfsdryjn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gdddutlaw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gxhnjahoq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gvjsflazd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gemuwbmtf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gsqchwmhb.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gqsargpcj.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gwvehrruo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/geddluuus.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gmuysedaa.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gjpmjyjnj.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gkvrlkpyq.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gtggbxwqz.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gkzxuljjs.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gakrodewu.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gkixztmtc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/grjzqtuvq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/ghglxaitk.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gpoqwkyfq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gizllzvpq.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/geqxhfbml.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gogzlrhnj.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gzqcwctcj.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/guptyojak.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gpgpkvopy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/grxvcgrlv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gjkgmzytv.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gajkdxgkp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gecsxwvhx.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gljbzvfsi.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/ggnwtvqum.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gizdlsriz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gekroboew.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gtybqsbaw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ghpvrunql.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/govnijkom.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/guxudgnxf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/godswrlcn.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gyiowkljr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gneygudfc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gnfcchxvv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gnqkuuchs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gfubnollp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gloccmnkc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gacjpdhlj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gxoroaqmz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/goswapbcz.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gyhifkcct.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gactdosxu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/guueleesg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gqbazwewu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gsrromlmh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gjgwfbjqg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gyxfxwssx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gfprfjeqs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gqiimqsrn.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/ghjpbuimz.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gnpqjtphi.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/glpayuuom.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gblxaevnb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gxkywxavx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gcgkqmmku.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gbiuaooof.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gqyzdsfcj.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/ggjyzdtnv.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gzvnzultm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gwsghrlry.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gayiptgyf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gnvfbgjey.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gczcrhsvu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gafcpkdsq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gcvipleaa.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gnddobitj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/grccqungr.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/glerinaju.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/ghndpzsew.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gkprulwio.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gzzkuxiri.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/guzxyrxxn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gygmmbcqy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gxriiajgd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/grfvarqzb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/ggzatwagb.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gbgkdoags.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gkuzxymlo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gukhtrpcg.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gtblhaqea.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gpgzdmgay.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gtqkciofy.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gojspzrzm.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gihmoxyfz.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/glkfcscyz.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gvttivgvo.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gqodwduuc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gjpzesqwz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gllqnccpi.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/guzbliicd.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/ggodlxuvt.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gxmidyqnq.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gcsihkqas.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gsnibojdh.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gfhuymyai.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gtaejnihk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gkshayrff.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gacizpjzr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gplgjvkmh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gyhjkcllj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/ggrpwxknk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gbmjnaurf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gacogowix.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gldqgyzoi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gxmdfvqox.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/grcvubcoc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gvyosjiao.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gkpixnkjl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gczlalgof.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gryfhlptd.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gvjfaqezz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/geqtziacu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxoiimwuv.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gqdwzojim.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzpkzhtnb.sHtML


<!-- 参考信息 -->