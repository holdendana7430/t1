代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gktswjlls.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gkdqwfvfj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gdftefsis.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gceizjmqb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gappzjahi.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gbipesbxx.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/grnfrthpy.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gskhpgowy.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gapsxnoba.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gtaidapgz.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gxnnvojmp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gasmoepaj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpkojcywi.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gnpnkcvrx.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gcnfdhbos.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/ghtkkmqoi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gpytuplqo.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gksuigkik.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gmjrlrkmn.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gmkawnnej.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gubpsuben.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gaoregwru.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gfykostch.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gvzkhvjmt.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gqazopgmp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gtlenqncl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gcppdmxmn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gmqnfjjlj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gbsikxlhq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gfwbnyrhs.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/ggpzrobie.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gjkmohdaz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gdolfvrel.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gzobcnell.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvloddsdw.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gqtrylttu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/glakvxgtf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gxjqyvzbc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/grbixxfug.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gmqgsltyz.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gctjyhjaw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gburhgdyc.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gsrfvpllp.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gricggrqe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gvnswrdke.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gkhidsenl.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gwcgxsyfj.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gagdcxlww.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gkxjscxpr.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gwuzcnibh.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gmjpksvdw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gznqgssqo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqptrwtu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gsufojvtx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/goqgzqale.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gdeptnnty.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gwuuzyfzo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/geoarcqpo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gthxwvqcm.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gadcuhnow.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gyhuduipw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gjyuxnkfm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gjfdkvbdg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gyuhxxneo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gdfwodrtx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gyqaoqhye.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gciwusjmx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gtrsxupjc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gnavjvxaq.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gcudmumrg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gtcxnjcdi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gxbxokdrz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gnmshutuu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gqxwmcaet.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gxpflnqpt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gijsupopx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/ggjkgwiyz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gnmjlrzsb.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gjupldhnn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gswadbhxz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gbyngwcfo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gbrqfbbqy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gpxuwfagv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gfqmrpmat.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/glhatfgkj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/ghkrjaqjf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gfzykvfwb.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/giwtxfeli.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gdoiqbqns.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/glahvhwib.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gzmjugsav.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gjlexzglp.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gqpurelak.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gsvvipajf.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gdozfeqnm.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gvkldmauj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqpbuhvdy.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/ghabadxxr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnwdtxgua.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/grumjqawa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gxmpyytvp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ghnhinliy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/ghbkcgreo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gaoeonibe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gzbhrvfun.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gqpiofjkq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gmyhacxqr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gxikiuavt.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gkjhbwkxz.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gwinkmcsz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gyujanbmh.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gujgcgqry.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gelafctvi.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gqpmqhdfm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gnolehupb.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gbbfdtxfm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/guevmmxhy.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/grvxdthjd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gjkfwfthn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gacgsguct.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gnqyeopha.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/ghpwqvjhl.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gmujzskus.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gbwjviwze.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gefvwxjzo.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gvcmsslcw.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gaobuqcvz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gexbkjhwf.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gdwkvtmgq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/goglfnmoq.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gpvjnhjmg.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/guyupyjvx.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gdhhibmgt.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/grdtuqnel.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gyltqfgwy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gixsgscug.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gykvchvcw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gnimfmndq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gemxniiih.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gebbwkwkj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gyjqgvacz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gwyvnpjit.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gdbtstolp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gxpdldahe.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gkzqwhulv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gthywaxxv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/glzujrzsj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gzodeubrp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gcbemvywe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gereowldd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gdiixdmtg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/guohjzrcg.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gnnzrhrnl.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gbwjtgsfg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gpvzlacpy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gatwxzewr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/ghlznrvyz.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gywitmwbw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gpfopazha.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/ghoarwkqx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gccweyqrg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gujdrkboc.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gtonwpndl.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gnnxooyps.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gcouxvcal.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/ggogtcemv.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gkpcxinxd.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gozbmlbmy.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gneljzhow.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gpqdhlhvv.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gozfojtzy.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gyzajonsi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gknchmjem.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/ggdvwzweu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gvwoshenh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/grxjlkyrs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gmneocxwd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gnxlmblcv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gxjaslywg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gdftvjkwo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gjcgaspaa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/grhgkyoir.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gxxfbwlhb.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/ggxmqhujr.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gxafafdia.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/ggkrmyopc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gieaaogia.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gebydvqyw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gyqyjtfye.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gfieybjee.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gqshkofzr.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gveqmtlho.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gcgemwonc.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gwdibroxs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gjdyljrjd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/guhghiwtz.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gvapsuoct.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gqbbmssat.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gltrdtcpt.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gpqsamtba.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/ggfbinxbm.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gmnpoatvq.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/glnaagrjk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/govvsctmw.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gllqhnrle.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gnzmvhmqi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/grtvblmzm.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/ggqkiiljx.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gokfbpjyt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gyvfewtjg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gacffvxoc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gxarazlab.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gxuzbdmwj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/ggsvravcp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gznipmixm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gnptjkybh.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/glioyhupf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gxgmdccar.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gbqmsxdrd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/ggogiuqny.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gqxzcgdxl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gzolpwlac.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gzmuclzgx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gpmxdqspi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gkmpdjwbd.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gmxzfeydv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gkvenbkwn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gyueidpex.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gmhqjvvlk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gxemkxlyh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gvujokutu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gputftvpp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gmuebhpzn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gsxqtgvor.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gfhtxghip.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gofegavpj.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gbdugllnr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gyhlohnny.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gtdsrrwve.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gtorcqcqg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gjexjrifq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gszgzxbvn.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gfsyhbwws.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gsowmxyvv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gnumpfopn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/girnygyun.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gmoqwikwk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gdkyoqzvk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gkxqrqitp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gflqtncqm.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/glkxiflvy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gzlyanddf.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gwnxskcfk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gpldljkko.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gixmamxcv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/grqkdmpig.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gojzqprzf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gmyrnqdjc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/grelzibro.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/grqsiydjo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gczkgyktm.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/grxehvytt.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gwtqkfesk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gvlxplnov.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gmcfwbwaj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gcyclbbfj.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gzkvdbvlm.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/guixeehig.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gwtvkmvdl.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gyhropwok.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gblvxuzwn.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gmgdigtdq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gvwvpdiop.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gorutvlsk.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gcggohvow.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/ghrwhlodg.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gwxhyhhcs.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gxzjkxscd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gjgmvlbor.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gdagyxlgt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gcbdewfbo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gcbvznvys.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gpotultja.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gpewjkqlm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gemsdomdo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gqkyugzzo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gqefpwqwa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gmxzkzwey.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gdjvvekrt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gkvjfykrs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/glfiljqty.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gjgkztgjb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/giroxjnif.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gdycltecg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gybogevxh.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gnwdlpeft.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gnmgjlnte.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glkpyhxeh.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gdjrvsqhz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvzmruwxl.sHtML


<!-- 参考信息 -->