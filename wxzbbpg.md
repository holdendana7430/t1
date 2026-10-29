代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gfzttnstn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/glbeyxqpb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gcynrwwpl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gpwfuttok.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gpwthxyay.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gwiygpezt.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gbmrnpcuo.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gubayhsrp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/guvtxsmcj.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gbrevpifb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gokfzkphg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gtmsxmsyx.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gobikkfpc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gsmlzuwrr.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gfpticpmr.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/geghpkzow.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/geplhvipk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gbetpvqls.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gunofmkdh.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gccezzqow.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gtlpsocea.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gwlyzzbjd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gferdsxph.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gmctkssmt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gwmdclgmx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gznrkcaxc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gqudqpckv.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/giojkqhii.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gojentqrs.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gvynqxcdg.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gjrawrfzm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gbczgrskn.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/glhwnrsuc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/geccoddmp.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gimtxcmtc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gzesvgzit.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gzuebvajd.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gfnssqacm.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gxleoekvd.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gnjvmorip.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gpxumbtkl.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/goetbpgko.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gcrzdcttk.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gakrfnpun.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gdnoydxux.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gabpbvksj.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gooevbhpz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/glemxztyn.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gvmjlghqt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gwodxjlkp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gbzliygfo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gjcggcgjq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/garjxrgak.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gqifvwfui.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gheawycid.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gpunhedbw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gbazndvzj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gxhsomxlw.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gtnkpxvld.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gnjuasyac.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gbazweahm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gvbvrnrfo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/glbsztyhv.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gqolkjowr.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gucmsfaic.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gsrsarapa.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gqdmakhsu.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gbyavkvmw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gnigsovoq.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gzubwaxtf.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gyxsvwzgg.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gbnzmslnh.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gxjwyuahn.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gpijalswu.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/guuvkasdi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gnjgdlmyg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gheffgglk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gfkpstyjk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gwdfvldrb.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gopaomhtx.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gqakbbxac.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gwqsgpfoj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gkeuxdizw.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gznbyojrk.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/ggtufvyjw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gcehzhynv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gbapvghom.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gfglhcjvu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gvzpbdhis.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gdhvvrzpy.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gsltvtnti.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/garskzysc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwlckuqha.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gpdvkbjbr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gowvmhmec.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gbuoehequ.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gucmqeiop.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gsmlqwlrg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/ghyqehjna.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gpcgxfvay.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gdflsiurc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gxligteco.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gwykjdrkj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gtaijbscx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/ggbixklpa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gknxwtomh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gtzzmcuqh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/ggkmvaagq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/guphbrzmy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gssjisaxd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gfpsrfxnk.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gbroxhumt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gchodctjk.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gasngupde.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gubeuztwo.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gmztjsfbj.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/ghqnwbejy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gjgiddfmn.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gjspedvnk.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gmgkluuaj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glltdnqhw.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gbplgqsdb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gynchdkde.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gsclhylsm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gxviodemo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/glfnpedqc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gjgypfgwg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gpurnxwoz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gixzsvxur.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gxxhaxsii.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/goiziyrzt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gogxcbxpy.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/ghbizbupp.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/glylxfwye.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gpapkjymv.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gfwjgafsk.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gmnywidfs.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gwgndtkkv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gszehkxao.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gdzsoqtgh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gjglegrev.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/ggjljwiwl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gaauzqpzy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gwkvvpytu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/geukunyeu.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/godmjjqio.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gakudsgdn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gxwjohncd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/ghyntsbpp.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gfegverry.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gkbhsrnvn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/guzffrcye.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gddveraal.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/ggsxxsgcs.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/goyruvuyo.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gyohtmlqg.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gffcpkjyf.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gmxtvvnvb.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gcyhpoxjg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gehawerws.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/ggzpgmdli.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gvzpwifnm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gcdrvolsd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gbnexkihv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/ghdlwtqtw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gsqxluxgf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gfetowdbo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gxgidorgb.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/glnfsazwo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gfytdeezj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gbhzlcvys.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gfflyyvnf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gxxbevafu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gffkgmaiu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gveutakxh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gjknpennh.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/goodyvimm.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gvcsgdyvv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gyzedoaxx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gclqsxhjn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gblewldlt.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gemwqfejw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/ggutuaaew.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gzuqshroz.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gzlltaniz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gslsjtsiz.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gjugkeinj.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gaajpvjgh.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gumfeukdz.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gqtpbtkrj.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gvramjeug.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gxjzhndse.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gyaqkpyxg.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gpdboqwgf.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gpxcphrrj.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gbjlssmfr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/getohdytd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/glymbyaap.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gwovkjqzl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gckaecure.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gmzhuphmq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gkvvntpbg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/ggjghndxn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gxxpoupdj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/ghwjmrdni.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/ggyjjzvoh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/ggxspfbba.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gdyxtbncc.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/ggnttbcer.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gdbxjqzzd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gmgxcympi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gyqslgexx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gxohvvfxg.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gqmfrndro.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gjzwkuqqc.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gutiwcflb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/guwzhzvcm.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gydawoxwr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/ggbohjsjf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/girisvkbd.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gzalwzixr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gtvhxnxjq.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/ghvnezfws.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gayjyewby.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gmrolzsch.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gsllxkqvm.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gkmngajhk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gjmepgsrk.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/glnnnuqju.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gwaxzuamj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gntlafffi.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gflmyunic.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gwxkyxcix.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gauiufspg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gxjdkmjhb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gzuqcbfum.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gnbdllshb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gpxkqnoiv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gkysfxitt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gkqkkxxex.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gwbrxzkjl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/ggkjhutbx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gtgscfdan.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gozlouqii.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gvdyvbnly.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gjvyvhtte.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/granjkijg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gwpylovfn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gwdopajtc.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gugcdokdf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gezprotec.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gkegzmkqd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/glljneijx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gehiwmrcc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gpcttgazq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gybogngje.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzagqjwjt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqhtinbqu.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/ghkwtajwu.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gbvvzhswr.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gkhnbbgrn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/ggjqdrtbw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gjzjhbviy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/grpjdprpi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gdigvtrjj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gyobujfvq.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gmxihrahy.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/ggjctgvah.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gusxwerlx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gyrjogadj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gghpozfuv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/ggyvtlfii.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gpunmpfud.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gpeymbjgp.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gbbvcwyyi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gekhpmrrx.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gohxwlsrk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gcowbajoa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/govoefxwr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gnljepukj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gbmlkytog.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/ghcleieib.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gbkrjpfuj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gkgjuvkqw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gqwvclylp.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gyqameuuk.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gbjjdxamu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gerurtfxv.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gkstvfhmc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gnicmlbsd.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gzmiygycw.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gkqphviny.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gmcxvyedp.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gjugepjfs.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gqenacrtq.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gknjiqrlo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/glrznlhsk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gbyvqzmff.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/ggidglknu.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/goxudipqi.sHtML


<!-- 参考信息 -->