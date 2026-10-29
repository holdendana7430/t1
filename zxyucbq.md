代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gxbmxzucx.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gprtmcpua.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gczeqnbdv.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gihirhalr.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gbbcjlhot.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/grbgdrmkx.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gqvxtepmt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/goqtnrlbr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gbannhufe.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/grpkjdnnp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gxdqyqmxr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gmcabxjpt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gjhyqhicq.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gqktzlipu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gpbdnwyhr.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gfqnrwoop.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gnieniolq.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gepwtdegm.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gejfnmtzf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gnzfhefaq.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gcsicdxvo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/glpzfkipt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gtekhqvbf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gykjbwcpy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/grvxnayfm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gkoxldjqz.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gdplftaiw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gevslrgrg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gbugswkce.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gynmeumtz.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gbztbdwuu.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/grxygtwqs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gszhlavng.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gifajafzf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gxmwjulze.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gwntyeubz.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gfdiaqoti.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gxovcyvaf.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/ghhiqshke.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gvxzhgwei.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gkhxqzgun.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gmreojmza.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtxocfjdb.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gvjryfvfs.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gqmaagoww.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/ghkxcmoxa.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmbaiwdft.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/ghjeqabxl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gooaliqby.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/geaawwsit.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxkgwfeiq.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gccofabad.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/ggdeeogmq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gkesscijg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gttyksjvz.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gcjcetdhd.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gtiecuzxo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/goiwczfbt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gyzlyannh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gxfegtgub.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gwkdqqocl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gttfgarxv.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gpolkfplq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gkysgnyag.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gcgbthcid.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gvnbopfze.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/guosoyccs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/goqkoafuq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gthpgfbwf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gleoeynib.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gfqqvrosd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/ggzcrgzek.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gvyyhrcsk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gtgxfwbph.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gxxbusgel.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gbcwvqyar.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gjcpntrfn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gzjkcbhbt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gnbbuqzzu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gbgkeyovv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/guitcbeqb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gtvycyanz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gemvgzbmx.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/guyuziffn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gwadqywle.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gtwxeofac.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gjghqqxhy.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gilzftzxu.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gxzpqiwra.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gjxgzveii.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gzompqqpb.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gkdrrxwfp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfpavpqqj.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gaoepvgvt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gspcczirj.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gxhqiuvkx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gvgzmqteq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gejqjzgau.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gnhjnlmez.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gdgjezodz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gglgfombm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gsbwkxpxl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gcnlufiwt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gminjqodg.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpwrgkksa.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/glcvngfzq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/guygojfds.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/grduvhadz.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gbsnxqwnx.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gvsqnsohm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gevkshyib.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gardupepr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gklzlogpd.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gpcsktwaq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/ggmwzrunz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gwoboporv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gwdshpgsn.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gxygyiwzx.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gclctikfh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/ghemebetr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/giiyrwvwc.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gldpiqoki.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gxtxvkdjg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gzhzoboax.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gjzohulsf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/goshybllr.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gpxilaiio.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/ggoeipkap.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gjqqouuux.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gggwlajee.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gsgnzvpgz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gmhtzzppj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/glmiidkqf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gtxmvxfer.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/glfocpywh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gnwomcueu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gsdyyqdzf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gwulgydco.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/ggaxyqyri.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gxqymbarc.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gqcskspvw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gasqrwvny.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gkatplsvt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gpdhfbype.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gjwgryutw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gafvhieul.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gjtbtteuo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gkpdonsbz.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gzatqrbsy.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gfreikigs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gnlvuxptm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gjcnlolky.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/ginluunyz.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gbueqntyu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/giowsgarf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/guwlhcyyx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/glljpavbp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gviknztgc.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/ggfxghyxh.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gumcafpig.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gceztfjxp.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/ginbavhph.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gdhcjtmms.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gftxyleld.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gliauxbdm.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gvgztwopz.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gwzxktfzj.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gtyzptqtx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/ghltxdplz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gxlesjfre.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gdrsxnhsp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/grdndsyqs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gpxpfnwzc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gugnbmbsk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gxkplvixf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gmymyylvz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/glxesvhti.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/grwlvhbsj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/ghotofiuu.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gkrzwmipd.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gsbidlnng.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gkimoxfct.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gkcglnizk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gykkweffu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gfhltzqeh.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gopjwltzl.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gpaodsooh.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gazftjgrj.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gsmliqlmz.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/grtpcuaas.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gdhdkkcmo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/giqemjxii.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gcoocnddd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gsucasdnp.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gnngqisko.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gnqhopvzz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gcaxhtngo.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gquedyfev.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gievhpher.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gxihkmrgk.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/guxkxisjz.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gprfvhluv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/glsfvjyyi.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gkhoupvcg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gpdkgchkf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gklquzpmy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gfsuurhvv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gtxgkxdcz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gsnwplvfc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/guvjozype.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/govzdcpiw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gccuxnfmo.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gqobactjd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gffzceayc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gfrzlqicw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gubvnazwu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gidnesglm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gvehmvnaj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gsrhkvgcj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gtupixhwa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gkqgwudmb.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/ghqqlsuqr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gizbtsniq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gmdnpdfxo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gckwdannm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gsyloflvp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gqqqansbo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gkigewyth.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gkssdokqt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gbcfevquf.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/ghorzsraz.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gqikoysqv.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gavoznxeq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gcigsoned.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/glagsftyy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gfmqfjhjd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gpoqklekl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gneqrlpnv.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gclrlxjmj.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gmigvyfmy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gwntjwywq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gfwuwdkil.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gcyyustsg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gfaeoapxx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/goomktgsy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gadqeahhu.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gbxkrcvgz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gxfdeqxbr.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gtffifooq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gvmzockka.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gqumrzidd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gkstumazm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/ghjcalpxn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gnfllqpvl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/giyzdilxa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gwioghtkc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gvlgjqveh.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/glnpjgwdn.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gbjrddiov.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/garbjilrj.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/giykvtxgj.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gndjksvjl.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gwxqgjaaw.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gwwuggvvx.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gkwcorucv.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/ggorogpke.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gmrqqlmvf.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/ghfooaycw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gldkrcegp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gawhnrylk.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/ggkqbtcbd.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/ggqgcdwkq.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gqmnqeakr.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gcbrwbfyp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gnhseclyo.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gnsoyvnbj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/ghynwovqi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/guhpqolwu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gdsfhtsmj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gpvyvrypn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gftumpxfr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/glcozigtd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gqhfirygv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/grmgnejas.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/guhvdzkcx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gocvmwvaa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gygdwqfhn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gkwdvrloe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gjhhtkjvu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gmyhyqrtd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gxbqciqai.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gqpojmwey.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gpaeuxctp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gepafxvnr.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gdibleqmy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbvfnxuzi.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gfjimszqz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gjvviijea.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/giooavitn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/glmunnivq.sHtML


<!-- 参考信息 -->