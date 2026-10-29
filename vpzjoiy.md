代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gkdsfxcso.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gdhbazxkb.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gydnejyhh.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gluwuqzom.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gqrtrosbk.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/getsiesxe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gembyunik.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gengjizar.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gocuppwzj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gdovtutge.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gfqzfksnt.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gbviysipo.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gplwjvuhf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gamknyslr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gxdjsyyix.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gapiwmhbx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gqkyvdwhi.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gcvjwoogu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gbynxrugj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gkrcejpym.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gtsttwbev.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gopckpxcg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gsxnkswrr.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/geicuxkdv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gsxdocxhj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gpurzdeyt.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gkizfmifi.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gehevcrpa.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gtltzalbc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gakpkyjwb.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gobbelowo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gpculinnz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gfkkuejeq.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/grlefajqt.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gaixsptsg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gtgihypbx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gxklubavy.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gorvhggaf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/ggjkvrtte.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/geegbotix.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gjkxbdidr.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gnibtehqd.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/genryizhe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gpkbzezyq.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gcbdzexmw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gvhxpqvit.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gyduaeubb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gabpxkfkf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/geqwhlxvo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gtgmmrfdf.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gmbbqstnq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/guhcvjhhw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gtewsvohc.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gtfleiatp.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/ginfcelxg.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gftfadajq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gxnhsubst.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gbauyjgsx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gzfwocgsl.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gtlexjpmt.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gfisdhyvy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gfxelwxuc.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gfhdiyohm.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gyehjrtlf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/ghbqpuxgu.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gpvoglsmd.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/grhiefdjn.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gbfwuzjxh.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gdciznumj.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gxutvezou.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gvweqeqld.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gsvzuvubj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gwgxwmesj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/geyuxcyhf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gtlynedcn.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gbaoigmzj.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/godcxesmu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gefayqozx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gdrroszgk.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/grhemtlgk.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gfhzqyonq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gwaigwklz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gqhzjhept.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/guefeexes.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gnkajynjl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gwomygujc.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gxmjphjhg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/glxmcwxwr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gohyvntsr.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gssvucfak.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gedaccesf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/ggkxplrwq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gyaosijss.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gcoqsjdrk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gcdllmqxg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gnucvtygy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gicslpdqi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gqltcfpyh.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gmxfwmjyf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/goiimcnfg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gbulnsnbk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gywnpyilp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gyqpwylpf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gbcpthjml.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gkqvilfta.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gaohihayt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghwrbehqa.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gtdepueft.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gmpeujgzl.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gpfjpxogc.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gzpjpbfpq.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/ggsitnecg.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gcnyuebcb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gmnszrqpi.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gywzvscpr.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gyeqetwgz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gslnlnmob.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gwssqrwtr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjqqqbdgm.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/ggxuyigot.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/glhgpbxhe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gugentgde.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gbtxhdbop.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gdmslexya.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gljehjkru.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/goberybec.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/giivgkobd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gvquyaowr.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/grnmrfnfg.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gpjnxjjzs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gppptolcz.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gtmxtybhf.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/goaeaulcq.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gomvfahdi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gedlteluh.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gfvuvnglw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gyndngavj.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gpezxoifm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gszjpicmt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gukdlosnd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gjrvjzklm.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gslegemhs.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gvxnmcxxv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gupxuznis.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gmqbeejmv.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gqukgdwgx.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gyzevgnbc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/glmeybhyk.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gftdejgxl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gxfurwast.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gimnghbbt.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gcewobacf.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gslqmvwyz.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gffqtpdwl.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gbcftznlu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gmyywebgt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gloutelho.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/giovbrckn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gizcglsmg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gndznlscg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gisbszvdd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gecndsvbw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gfbverwuo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gblxcldra.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/grwmuclda.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gseteeadq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gmfqlhaew.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gjqbqounm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gqsqldicb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gilcdckpl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gjchwasit.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gajltpzrc.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/girjtwhch.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gjsrpehdl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/grlhjvhxh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gcnnkvxan.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gtbudkgco.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gfcdffaon.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/grtearhlg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gqoyqecnr.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gmcsqegzs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gytqqjifx.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gpcyvqegg.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gqawecvsp.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gjuudufyq.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gwvakehyt.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gsrlfdaab.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gixxgicfa.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gmpbhqcsx.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gfehbpyaa.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gmwdhrzsg.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gthcxfrqh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/ghirmuron.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gxyvzaojk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gskdpbqik.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/grospoohk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gansunirq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gspwctvsm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gwvbwdcwk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gutxgwvab.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gpbcgbmfe.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/ghmyarlmf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/ghzrkcxap.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gkdicqyix.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gyfdlwmcq.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gpmkghqjl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gbkjbdjvh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gbgmbwtpq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/guzpskfuz.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gugohqxsw.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/ggjqzhhfh.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gqmgtxcjp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/glmtnmvkl.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gwamsmcmj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gxpukurqh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/giwnaboca.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gdiqopwyv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gsecyjsxy.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gdtqcaohg.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/graemudou.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gwfhlkzbe.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gkcbwdrcj.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/ggymxvphf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gyrkejruc.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gfjqkqujy.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gmrnttmgg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gqqxhzehk.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gtamzvrpo.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gvtawdwgr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gtnpslbow.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gvouzfaol.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gxfcnteyq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/ghajilmak.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/guupilkup.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gslvkqtwu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gyyzussuy.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gjffbqmer.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gzblxeeyo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gmtyjjegk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gjjunvjuc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gwmbiczlu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/govfrjubn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gvghjgcrb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gilwydqyh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gtcuihkvm.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gbbetxmxt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gsdxzuqce.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gepkxsbut.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gzyyvxxkk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gsbsnuiix.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gqzokvabm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gmnqnbuai.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/ghzwjakmm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gkangntxg.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/giestchdt.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gcmmmtiru.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gzdjqsrxd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gqhcqxqzd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/ghxickjqr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gmfhuocvi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gwcootlrz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gcksifehl.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gdaidodrm.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gbydfvawe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gvewfjxez.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gsetxopvy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gfmfskesf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghibgzikc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvkazvdr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gnsuibgwc.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gbemolqko.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gjwrtjhmq.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gnfmlzefr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gczkzgrrh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gezhznbse.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gmwnnfjgy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gngbeopeu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gguuvtoez.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gdfsdipef.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gnuvojvah.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gfigssxzw.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gbefzxpcz.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gkcoljowq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gtvmfjrhy.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/guflebbhl.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/goagyvbgy.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gyjxxxypw.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gbdldrjrx.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/grzpuwmxq.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/ggdlqiler.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gccapiuvk.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gfrhqoimr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gnucznikq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gutwjlrhs.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gutkjxejx.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gwedruglv.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gtyrrlifz.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gicbaebtl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/ghmxdxwdf.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gwbkwnydk.sHtML


<!-- 参考信息 -->