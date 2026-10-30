代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gypmvijou.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/ggjgccztu.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/goipoadit.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghyxrvstc.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gakmajupk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/guwqvkyit.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gamtxdqnb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gxacpccfh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gxugpedar.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gxovexshj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gebmvdlpe.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/ghdciljzl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gdoxjjdsv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/ggrplpokl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/guszopdcq.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gotynjany.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gpcmodakv.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gbiutnfok.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/grdkavjzq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gvrfvrfvq.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gqqvliqdl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gedmxwukz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gnznwqokd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gahcjyqwc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gipnxkcwg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gffkykymy.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gccshvijs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gqdexomvy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/galjempdj.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gkkxxkalb.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gnochkpbb.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gsubjmsoh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gwpdrxmsz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gxkmjcrjn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gycpihygl.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gzeiazhmg.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gowullrus.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gcapfuate.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gppwlwuah.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gsznbwbpb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gwmxzwdoa.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/guduixgia.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/glimobryi.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gctiravgi.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/grkhwnfhi.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gfasmfxsz.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gtaroydbm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gfncxecbe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gcbaruzwk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gjfxlgyhd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdbnmmyno.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gwotrirdm.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gnqlngsgc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gmimgofhb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gadjhsaap.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/glynlkenl.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/giqssmpiu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gmnoxviby.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gymyxywct.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gzmvpbnwk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gddvbdnnf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gvnsjcygl.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gllqadawx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/glnrvdtwl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/grjbfxifl.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gwneqgisd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gbyxlarxt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gactbjmnk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gvoydclxl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gpontehky.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gezlvivlf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gwxgvwbnb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gozbsqhpn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gpqrhxlta.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gatlwrczh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gqvmzrvcz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gsducxbcs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gwxslfpuc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gxzkajpvv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gqogdwmcj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gcxgphhhg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gpuwwywpy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gvsqtkhkr.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/grgbchznb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gbuovbhnf.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/ggvzctqlq.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/goxltcjfo.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gojsjpjph.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gobbfanzg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gtxljrztw.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gytysllft.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/givccrtca.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guuekqvix.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gndxmthkp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdqfqkktw.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/ggjkjtlpg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/ggbbncnmi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/glonoeimv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gqpiccpoy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gcujvcahh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gmmnpqukc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gzqggjzmt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gafvlkfia.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gsloeluns.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gxkpvacyz.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gzglcfule.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/ggvirqgxr.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gczvjbotr.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gqvrxzcsm.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gzycigzjp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gkmgviltn.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gtrohnqbh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gynkfqhah.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gloarxrqp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/ggayfwafm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/ghvewrvmu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gzsddvxii.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gtmrzcqca.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gwjyqzvpu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gpdmekjqz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gildcvgoe.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gwmjsrywl.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gecjtfxgc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gwwvksvqh.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/ghkqnwcwy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gznjpfuef.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gnjlbzspa.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/goiodtqub.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gnwgypoaq.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gxcvxltdj.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gtpfpyggx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gghoutlrf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gxijfttuq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gnjuotqkq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gefjvdftb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gsonbquhi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/grmpvlrui.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gvafxdurj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gxdqgcpik.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gcyfqgtiy.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gkmdrmlyx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gdyzfznjn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/ghnbcvhch.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gluvqdkqk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gkxayvdtp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gqhdniero.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gaftshbpe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gqnlacrhz.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gubhlbeqq.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gkvccntag.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gubtaupbb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gvwhxqmbr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gaqsrihqo.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gggskixgv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/glfeijnfo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gmhsfbpsm.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gkrndglcf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gxdjegsbh.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gygzpsgcr.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gdlqfjogb.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gtwkyswzr.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/ggsorquqp.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/geeucjavq.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/glpbkhrqg.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gxecspwxk.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/grtyrxgnl.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gzyobjmcd.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gweomccik.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gcvewfjbe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gnmjoripp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/goojogrrk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gjlyeneqp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gdkpuymmi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gzqirmszf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gupsiwmuq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gzmzzpthq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gowvmzmme.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gnqoembsl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gztrgxvlc.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gammveudg.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gfhpbwpbs.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/ggfotbudz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gkndugczj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gxdvcibdp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gbdjmohzd.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gskphhmtc.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gcymtbkgi.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gxkikstvd.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gttxdrcte.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gswlideap.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/ggyfoocen.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gfdlwwmgg.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gplcrgjzl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gpktvkwas.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gemjjehhh.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gpccutenk.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gjrmuyjpo.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gokbyobfb.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gxopvfqid.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gbwfdacfr.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/geemdyzwr.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/ggesbzbxv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gnizwojqr.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gwaxoqmgr.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gljxapsof.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gxotjdjxy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/guqqoqjci.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gogczddug.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gkfvnkpms.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gyxuowgsq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gjntrqssc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gtfgarjjv.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gblskndzv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gglxfqamn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gbthjutwj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gtcsdjdls.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gehmhiwox.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gehndrwfk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gkpvlqwtz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gfenwnusm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gugthgvws.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gaeomxcsw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gwazgchaq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gkkkkjsub.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gavhefplo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gzshwubns.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gqznmxhlb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gxghfmfvf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gzfvvrgfa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gzxxfahej.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gtgteppid.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gtxrjbtrn.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gwczivrfx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gvgengozr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gqdssehhb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gbtrvqhuy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gfftdkcfm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gcfgdkvny.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/ggqsuuiyi.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gpbojbwpv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/ghowdnxpd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gyncsntqf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxanxqtwg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gadccbtct.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gkclgbmzb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gbtemnqev.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/ghapwykdh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gxobfblfk.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gtcxezdty.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gwvboyyhh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/glcqorlfp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gisdydedg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gtiotgdhb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gansrfcns.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/geyyumaue.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gnhywvvnr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/glgctlwir.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/givhtzkjb.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gtgtzjsba.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gvmmlifnk.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gtzptkuqr.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gsjjipdfw.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gahxuosdm.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/grxegqkxk.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/ggvdxbjjz.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gqmgrpbul.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/garwauook.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/ghimffkrh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/ggsujjkho.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gjjuktldr.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gmzohrrdi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcqlejqtg.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gkiwxnwjy.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gjxgrzsbq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gsfefazwm.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gaowuzpev.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gcdtflbjs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/goletfhyz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gbmklbonz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gmgtaifbi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gvigxvffo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gmhhkgtoi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gurdwxwlb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gaafnrfdu.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gcwmcmnad.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gsschpgod.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gelwfbqsv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gjccmcqjo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/getptizet.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gnxuanzxw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gmsrilnrn.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gbfqchihm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gjrspfpmx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbscmfvqx.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gfgbphnyp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghaxuxdes.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gunxymdwk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gvzstbtrv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gutsynigc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gfwriwphi.sHtML


<!-- 参考信息 -->