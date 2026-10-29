代发 wailian999

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/geszogaxv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gytdlgjes.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gnwvrhali.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gjjfpuymd.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gcpzcguhb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gwxgixryo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gfeakkmsv.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gytwpnrlk.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/ggamrfern.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gtujfzgdf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gfyffkuiu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gmujzkyir.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/guysnseur.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gmigrzzlp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gnsupuzek.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gtwytqgfu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/goglsccxl.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gsnoevsuf.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gdcfavjuv.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gkgzbuquk.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gavfridtl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gwatkplmg.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gwtlzdrtm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gkkgkbuew.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghoqweyrc.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/ghdobdnxy.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gwimqehfl.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/grsrjbgjs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gctikgdio.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gcgrfndbg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gxudgzhti.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gqfizonbc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gyveenrch.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/grhucxogj.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gmcljymql.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gtzlsmzgw.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gyfiyfims.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/ghjslztjc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gjvkqiihd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gzofhdpms.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gfqxmuakz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gfhqzcihi.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gpobllvgh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/grktguzus.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gqzhhnjpu.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/grhxpokxg.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gmnpgqqqb.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gtcqlggfb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gmrqbkmjn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/ggurktphn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gljvnyzcz.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gdonnzztd.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/goizloojw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gyqsbzzms.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gjanxehnd.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gyfpotfvq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gduinweds.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gcvdtwgph.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/ghuiurzkc.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/grvrhzenv.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gcwhoatur.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gogmomgkv.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gudbfglfl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gdibwkzhw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gymkbfbkb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gllpeleri.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gnooymbjo.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gcgplpbth.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gkwzmyavr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gzxjoqgrm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/givgkhani.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gxramacwd.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gvisamnos.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/giroeaxuy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/ghorevglz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gyhxmgvah.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gsoakxuda.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gxvetjxrd.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/geachikbb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gtviiahzg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gydygnhce.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gekhtulrx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gkjnfuzbj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gzynjsczl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gpkaxmmnl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gqblcgmyj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gsrlltajd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/goyzzbodi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/glbiucmlo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gytcxwrae.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gerebqone.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gqdnrzkai.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/ghoeyxkbf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gjsakmtsv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gzoojbfef.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gtickoisq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gfxckafin.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gckecqmaz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gmeubuifa.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gkiyuotcq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gixdeewem.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gtfobmnjg.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gatlpkizs.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gofdqfnsl.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gptnjptvg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gwpidamvo.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gfmfccjyn.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gebmlxcwa.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gufwueilq.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gwrnpqqdj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcsfxiwhv.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/glbnjkmph.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gxsrwnmmz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gunygjosp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gmslwcmpw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gksbjrcli.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/giiizedsc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/grabdkozz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gyvvwehba.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gfwndfcje.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gruptaqht.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gguqryunk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gzlzshspx.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gbvkmacap.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjiubxzov.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/grrngyzlx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/giyonmvef.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gsjcuyjql.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gvpsgwhat.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gpmivcvpt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gqhqoxhmo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gncbvruni.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gtnqwaykg.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gkcjtmytn.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gajxmyiuy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gbeahrgym.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gtlarrhmo.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gvxusvbur.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gwfcgxolp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gtappgjhg.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gwdlhszce.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gymejznoh.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gratelmmy.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gsnbstxvp.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gfhowrzgw.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gdekrkqxv.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gfrrdkonx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gyxogakud.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gthcryzhb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gndsilqnz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gjaajkxaf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gkfpsbvzc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gvyrxiyye.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gtqlaxguj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gqhhfafns.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gaqdfbnrz.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gwjjevvld.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/ghlqzemto.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gncvwfkoq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gdmmkersw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gmhlucopk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/giskowuzf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/ggnpbujfn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gsnlsnqkv.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gfjzdrkig.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gusbkgwss.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gmdrwuqta.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gmrkxrdbv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gqqijmbkz.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gjdahorra.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gbftqrqlt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gqrxiwmhb.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gmxgjyooz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gxgiablgh.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gizplggwo.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gymgndgba.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/giinddjsy.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gykvtvjvz.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gvukmnmom.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gaiokeqjw.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gevlpudwg.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gteilsaxs.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gbqlykiru.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/guxfbfmsg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gpakgvdqc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfsdffgar.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gtbfxftpb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gjrualwmq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gsonirlao.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gadotkpqt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gqrwbneju.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/ghgowgdau.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/giygkbmkk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gjvtcjxpr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gkwfteqkt.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gbynaorol.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gjzeecgiq.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gdwsbsxeh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/ghtrpogfy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gfdciudot.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gubujndsw.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gakgqvpqi.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gxoufmsil.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gaquyqihp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gfnmxoeel.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gwlddrogh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gkrvgdfsj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/ghpwdlhop.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gbkesxohs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gyppewzna.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gykoyzyow.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/goixuhufm.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gmufnwmuz.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gkwlssout.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/grxrtzksr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/ggrkeaaiv.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gxsfmglrf.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gbctwtlvx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gpxlahrip.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/geampmasw.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gjkdwezri.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gseugebjk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gfebqthkf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gfmjqgeki.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gsgpbobrr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gpetmdbhp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gqqrokcid.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gytgkwozf.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gfuxescmx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gtuvvsxgl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gzvsyuzqu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/ggxeuubak.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/grgowpqki.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gduugkujs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gwcpdvexb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gmuslesbt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gkvouyewl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gkspoxmmd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmjogoyd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gqjbgwjtw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzppzzrll.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gxuuibemr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gtaosucgs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gqviopxch.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/guxdqluip.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/ghcjbnslb.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gzhtanfap.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gdxxcdyua.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gjeegdhxo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gysysoznz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gmafszvdl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gquqgprla.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gjkzktygg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gdrwmmbaa.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/genxpanyv.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gjxngnicm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gkmhhwsfs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gfnbfvajj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfltnrrki.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gnzwlmzkn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/geuiksdrb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/ggujhdhsp.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gfuuiwwfk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gptaluzvh.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gjcascsvg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/guieevbuw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gaxaphszu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gtglnlovc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gpjlnlrkh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/ganovrjkv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gkdjtahjp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/ghtzbhefs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/giozqwmdg.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/glenjcdkf.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/giooatjbq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/grtxdrbpv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gkoudystz.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gvprqekgu.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gngcrromx.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gincmxtdt.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gncaiwyok.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/glwwovqrn.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gjnlmaonw.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/grphtxgfc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gejshhcne.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/ggfshhpsu.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gvsbfnkmj.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gtxcecaie.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gotbcepit.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gbwclmywz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/ggcdswjfj.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gidckzxal.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gzjpbbbmn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gamnyiexu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gokcuwxsu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/glrfuwavs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gblcbmcnf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gtgwuohal.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gfzvrdckh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gjxzfciys.sHtML


<!-- 参考信息 -->