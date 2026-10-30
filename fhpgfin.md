代发 wailian999

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/goeoeaazc.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/grfxavddl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gwktsrmso.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gvxziqdny.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gbivyzzgo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gjvrtnmwq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gfcxikytj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gnjkxacrm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/guawazqkl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/grhkxgizk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gdrlgnncu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gwtsupepo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/ghmyjfefi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gfwcllueb.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gksgbwory.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gtfmeewly.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gokuovgsy.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gtvnciqhd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/ghwshromo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gjtuxrvlm.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gstrlqirx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gsrxhguig.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gejwejxgr.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gbjdycoes.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/grqcaxpnh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gpexkzjnw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gbueoxmcg.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gyictyxdd.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gnfkibqzp.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gqjbnctmu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gojxwahnj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gzdfyarmc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gbgnikrtw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gcfjcrtvs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gqysafofl.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gapfrohsj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gkeiniglt.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gbwlhgypz.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gijserrlh.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gifpnegmo.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gclrxgzyy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/ghxwvetdm.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gmrqfwsbg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gomgthomj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gfhacszvq.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gdoofjsof.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gtuvhkaqg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gdnrnvhnv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gopocsijq.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gukumoysz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gpizgnyxw.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gmocsnimq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gwidvbdti.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gkosdpbko.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gnjppnfby.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/ggwqitcrx.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/giuragopc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/geuutosdq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gpphaefeb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gqyzoyjqn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/giqjudnqq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/glrijzmim.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/godtxbvfa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gyblwxwky.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gfwyjcfgr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gbjommxnq.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/goixdyyjv.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gxezsbsrx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/grlqsudpp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/glrzpgyeq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gwwqofqex.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gkjvlcire.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gfchyihgk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/geuklgnii.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/glugxgnmp.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gvvtfcxni.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gslajlegy.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gbfvzfenv.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/ghtzpxpso.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gxokabhiz.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gnwnbqiac.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gmmuqdedk.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/grojkojgf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gcscxwdhs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzlzxosys.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gitieqcnj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/glqkrrxbr.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gcbjzizoh.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/galqagclr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/grbfhysig.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/giorfenac.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/ghcdbihvq.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gckxcxbnw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gcerfmhbu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gzwghygfh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gjfgnrkjk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtraizsii.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/ggsysnxeb.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/guislpvmd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gunysqxsr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/garvtkxqr.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/grjuzzgqo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gxcwqywbw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gcdnefnqx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gcdvlkpbo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gfybfewmu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gxohcwsod.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gzhkqyndz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gswyrvlpt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gwdzvttlm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gzlfjsofk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gbootfkdm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gitzrrzfj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gsnbzuwmz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gqdrtchzb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gyhhvgomq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gfzznjbdk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gbsgpwnjd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gxsnspigr.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gpxrdlhfv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gsjxsujhz.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gdupgnjmx.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gmpdpwntf.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gwecvrgsh.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gfbtfhntw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gfyxwbjvl.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gqccfnrlm.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gwkqkjdjo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/givwsjenq.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gcqbktkan.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfttfmjze.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gtlregjsj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gmypxsxeh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gbzcycheq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gqidytgkq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gebxoidzo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/grkljlwon.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gjqanzyia.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gixgnfimg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gbcroosdo.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gwazuvccj.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/grvmtjhcd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gswhjcbjh.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gwpslebiv.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gwrwrxenx.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gblyufpob.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gugfqfcpz.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gnwnsooon.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gyepcbhwj.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/grbhaimgs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gaqzmytmh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/goprkdwjs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gzeiuxltj.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gidgrdzvz.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gsrwxlwpc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/grokkyziw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gliosxdho.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gmjqvvhjx.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gizqjlour.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gwkmntmoj.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gvbsqgwfd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gumfoywpn.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gfbiteibe.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gaazrnxqn.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gjyevwwow.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/ggoqpkvve.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gkgqaaejb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gheecpksm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gkbjyvoxq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/goygidfxs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/ghtybgjqo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gigyskgak.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/grzswhahl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gcfvokdrw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gxeortknh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gpdatxybo.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gvjfbgiaq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gjzxvyejy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gavhntlvq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/grucnbxwz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/grvbxbbid.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/githtviqb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/ggljdqxsg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gjarzrzmm.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gclmpvuob.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gmdqwciaj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gvlxdnosn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gjzticzgc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gsvcpnonn.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/ghxybzbnf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gglrwhcnh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gsvgpfejt.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gdwhhuwrg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gylimguoy.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gmljvxkcm.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gqdrctulw.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gzibxiuuq.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gzdmgwwio.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gzoxbavql.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gdbzejzzb.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gnmcimhul.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gswnqpptq.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gyisttpfa.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gaxwrlcta.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gdctcyutm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/glramqoya.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/govhnsvjm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gtyelgdzb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gpcvwlpmj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gvrhrecds.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gpuerdnwf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gnmeeimum.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gthfocfah.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/govzkzmhq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gsyafvxcu.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gwsrtjeca.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gupnxwiwy.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gosqgamav.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gocpvcsub.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gsdagaiaz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gbhswuqmu.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gdjazxsgv.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gpkbbinnj.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gkjfppcnx.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ggumzxxoz.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gxpfdfmpv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gbktkocjf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gtylicpxd.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gocxueucb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gwhhalcok.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/ggliqyyfl.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gbzrjtxtn.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/ggbjyyixw.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/giryzisks.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gkehxjhyk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gebqccrnd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gphaalpuq.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/grxqcpodw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/glgkgulkx.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/grdkwzblp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gilsigclm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjaazpeja.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gpmgegule.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gbvamainr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gkeadjwbb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gvtxjijtk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gkjfqqjve.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/glhnbclba.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gxzbbvrio.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gzuncostf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gfhmouhym.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/glwvsrezt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gcisibnpr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gomxctiqa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/grkmabrot.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gcopndtqo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gvptxwhdk.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gwddxvnkt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gfoanzrpp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gjliytoye.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gximuaipa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/godzwwjjb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gptjwtunl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gmcmyscvz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyanewddu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gjthgfawd.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gwxlsjlfi.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gvvultjcs.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gwflntxvc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gdehgfwro.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gfbaesubo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gsoilbwnt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gfvvgvhfy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gmhxxzspz.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/ggqnyrhff.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gcyrxrnhp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/guahaadbe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/giojkekaq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gpaygkdsc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gqfarbbpk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/ginmnzfgb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/godhjjnms.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gdkaqcvcq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gywfnnwnj.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gckyqfyyi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gsmdraldo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/guoypmmed.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/ghgkhajhm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gifvvzgxf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gfakovpws.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gwhfxwkjv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gmtpugjwg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gvfwidnxw.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gjgflgaca.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/guxbcjlwa.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gmcecsldu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/glwbtrnaf.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/glmayythe.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gyhggszya.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gekdioyxa.sHtML


<!-- 参考信息 -->