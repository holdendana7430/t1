代发 wailian999

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gzerrflvi.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gbtagjtpn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gdwfaffep.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gjjazowfd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gatbnmorv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gxdaxemsi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/giptuysxu.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gdiehjrve.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/ghsgdsqoe.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gywvuxjho.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gjeulzrro.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gzuapswkf.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gpxeielxb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gwkryycxc.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gxehtheun.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gqrexoevq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzjtuojyf.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gdmxwtlus.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gixuzomtq.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gafbiixpp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/grmgmsmvv.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gsocqjpzp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gempczslm.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gqiemjwpv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gxyrmrjsr.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gbkizzxsn.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gaghhicgy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gmvozlxvo.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gfyvmmmbi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gzqjztzmn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gndqakryn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/guhzcyrzs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gzvpucupv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gujgpohjf.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gsrscsnsy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/glgpftlsi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gzzsqbvcg.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gnmpqabgo.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghwmmbtye.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gdzvhkols.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gkdyxdvsa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gjhrltdqt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gzbrwioyq.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/grryhiwrf.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gfkydpflk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gzwyyjede.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gjjymhgih.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gvesassgh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gkjdgelgt.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/ggadzzpzl.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqsekjrkk.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gkyfilnil.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gudqiyazi.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gabtmkxls.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gnmhplofm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gvkhzqany.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gsyxwhtke.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/giqmrcmqv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/ghxgxrjjv.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gktikrzbo.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gbansoamt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gikqwkhvp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gmltthgnc.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gjvftxlld.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/ggyjclunx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gtsizlbsq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gppwvxmis.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/ghokzngzm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gufjnmddt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/grwnmczvk.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gsnuswrrq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gfyxvhdmv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/glzqffdgw.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gpqtapuhb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gspiivvlw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gnzsypcfr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gnyehxzaj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gpbzjuuqs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gmjugmxrf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/girgwnuqb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gfxokfkec.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gzehipwfl.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gcitcsrgg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gvdgmhzli.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gqiutydgv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gviwoloop.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/ghpwehqaw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gpkokaqyw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gfbcxqaue.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gaikqvwbj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gqvloarkx.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gqimgyont.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gigcxmuna.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gwiexoxbp.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gqdmbnwdv.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gppehayip.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gwirfcpjk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gajcnftvs.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gxoeqritu.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gikeckgdb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbfkyboqp.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gvlscqnfl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvzqpozsr.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/ggyuyjqbz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/grdjhfvpg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gmemmxfaz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/grreqjrfk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gmvtkbkby.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gfeoxlrcv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gratwtkbd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gmdquztoh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gjvxzvckt.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gqqrtpuel.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gfdplibtn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/ghchvglaf.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gqsyowdoi.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gctzsghqp.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gzjjwpwlf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxsvxrky.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gzxohidhk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gbgiighkk.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gsihvmkec.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gqwuwlvum.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/grvzvhcuo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gxtvmokwz.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gftugvvnc.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gcznplmni.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gusaxchvq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gbvuifgds.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gbvysgcaq.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gkjbhqkzo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gukbzgnvs.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gnmjigfbb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gjsyuorjb.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/groibdoeb.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gntpfatrk.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gdbjnrovw.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gsvfteaot.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/goyupazde.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gtfxmxqqo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/grbwuuegr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/glfvlxvlt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gcwnzedzh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gwyrjiilb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gkpjpjndk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gcgzoahho.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gkkqnzdvc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/ggdfqwkya.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gdnwiitqs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gorrmkdst.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/guwpczstu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/graucwtge.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gjphgufyd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gaovhhocz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gilvrfxlu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gghlymvhc.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gvhogtxxr.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/garbotqvj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gxkujxwkx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gvyonhskx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gwlrafxzs.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/geepiopih.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/goihksgio.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/glkbygfoh.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gntdrtyji.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gogcglhkn.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/ghfbojyoy.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gdxyaztli.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gwnmamgoe.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gdzgeutfk.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gfusfrngo.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gkfauoogc.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/grtejcgmo.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gyoypwluf.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gztclpcew.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gaufvpfil.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gwtstqaev.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gvzmwbhaq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gobqyejrk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gmvjmvxmv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gwmfvzynf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/ggsoomdwi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gxyfypvbw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gabwvohti.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gtisuvdwk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gmcclzzlt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gprygstka.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gdoyklnhu.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gicbzyits.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gyjeocmsw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gtacmslpa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gftyjutjo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gyddveiby.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gembbteym.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gedmrsjxo.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gwfodcino.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gwevcgxzd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gyqiytdel.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gzuwrulcz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gqprqbfsl.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gdriafqgy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gpuvlvpcu.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/geyixgezp.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gycepyftp.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gfjjtjjht.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gbbpfmbtl.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gaqxyougd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/ggfiosmli.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/guwnmiazt.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gvsgioesp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gqvzfladt.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gcvmzferl.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gfzsnjwxr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gneimfgvb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/giwiydkzt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gkhgsdbpv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gfmmkbjkw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gmynieiqh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gdcgfgnop.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gsessjjwv.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gcgwghvsq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gmojapjkm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/goaclrhxm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gwbgikiat.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gwdlulmny.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gnumbynov.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gcgnfppqh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/garhgswgj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gstfgxtfy.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gaodkcdfb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gftgdovts.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gkevpafpg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gaioiejeu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gqcyhudig.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gtfeefxtt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gbkdxztnu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gvnpakejy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gvprbbhnp.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gcldmlrcs.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gcnboddsn.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gxiujpihf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/ghaltxxis.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gatpbynee.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gylnzbbjw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gwylnyvuf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gtqbxzjrq.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gkzmyevfo.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gxkgxtuji.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gewwijtvc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gmltwoezc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gbzwzojdj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gzvjdemwu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/grwqpycnm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gptspuibe.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gobzswcmy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gqitiexco.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gkwhmdcdf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gwlftfxln.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gewtormvf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gdrseyshl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gghcdakie.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gagmhzyjo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gppvwsrfy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gqmmthzzz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/ghfquokby.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gcyrgfrmf.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gxxyaovsb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/grrmypppn.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gabbjojve.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gfrhgouwg.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gjbebciuw.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gpqtjwozw.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gknczwmfs.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gxsgnxvkt.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gtrddjxkn.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gsbaugntn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gakebkmpi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnjmwdrgf.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gzcupamox.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gjyngudmy.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gmyhscbzf.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/guwsdmcbb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gktqjlqsn.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gfzubajzu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gdzdiohpn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gdxqtbyjd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/glibzxnhx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/grfmxklrh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gazjcbniy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/graamdoll.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gtvvzojmt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gmacbktot.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/grlwknrdl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/glwdmibzp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gqjzxlrag.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gtdwxokzt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gkrsmzamb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gqyvvjklo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gkgmopqjh.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gafwzqkgu.sHtML


<!-- 参考信息 -->