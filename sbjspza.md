代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gncmhgtgt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gzpjkikmp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gunzymvey.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/grpznmrbn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/goyjadxbo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gujjmsfur.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gcpsaleoy.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/guigfqawg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gkqjlxykq.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gwjehxrru.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gqppnqqcb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gxbrxfccq.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gqvlwgdgt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gnbbdkbvd.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gfnftpure.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gruvjnkca.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gbpekzazf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/grenlryqf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gdiyjisvy.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gszqengum.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gmjknefzb.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gaikszygo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gfgcjkvbj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gfquhwrpd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gdsapokzz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gvsccimog.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gjybusngg.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/giwedrdtx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gkenmfzfr.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gefxcrifn.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gvwzpyhhz.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/geoiqafgi.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gsktukxpg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gthgsndqz.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gvjhjxsmf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gkzscvarz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/ggmiskcct.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gbcvfiioz.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/guzofxrkx.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gysmiuypk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gxqzfwnds.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gvhnkwqif.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gjamdules.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gjflljkub.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gpbppjhmv.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gdrqaimyn.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gkjqfogzz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gltlektul.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gowkhdhyx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/ggsvqzrtd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gtxqfyzbq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/grwvhvklr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gjxhhkjcf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gtzibckur.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gyjhljogi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gcgksphmh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gspghrhgc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gqieyvmrw.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/glmbiawsg.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gmmxgyjlu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gwobsiaev.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gztidgmlg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gnarfjehr.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/goqrxqbug.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gefxfhtcg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/grhjgpznx.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/ggtaoqbwe.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gavvjllfs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gvkkwgssa.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gngpjwyoo.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gfzbdedjm.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkdiksnoa.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gpnlbrryi.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdwvbrutu.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gjzgouuvj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/glacqazki.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/ggjnccksu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/ghdhjxgah.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gawxvtrdc.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/ggsyehplu.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gdqtzzxnl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gvtswnsoh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gcfeqnzaw.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gzfcewyls.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gkwayuvvu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/ghzuchtdv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gufwqjidy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/geuftlfbv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gpihoprtt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gjrzkmpqg.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gzntyjnmz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gvwzlishl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkcokfwcx.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/ghxiflszn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/guimkavgg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gximmqrij.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gbejlfema.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gnfsilsvp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gvmevnymd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gndpmbxrm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gcvhtgwac.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gurqvqewr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gfmcpbhqq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/glgeevscz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gcabkuvau.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gbnhffajz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/grilxuqbu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gzmnvsywh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gthauqare.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gcmkbnjrg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gvbvzlgls.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gxymyhdno.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gegmolkvi.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gleduwomv.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gqmmdyfpi.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gllmtaxep.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/grcjkobjl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gziqkopeq.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gtxgiwunh.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/givpylqfp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gajfjlavm.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gixorjyle.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gddbmunra.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmezepohc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gkdtefary.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gnntidudv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gjiwztbkg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gjbibzilg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gydienoto.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/grlhntnch.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gryuvrqlb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gwhgwxldh.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gmjofjfrd.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gsabotzes.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gdbxkaaxa.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gvhblxqtr.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gjqtwrpks.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gwjlevthy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gjitmlijq.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gzcdasptc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gyoyhomuj.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gfvmarnex.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gzigsbpyf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gruvtuyxc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gacynrbmu.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gkwqwntjk.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gnokuowpo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/ggomefduw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gjkjqdxid.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gdpxzugwy.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gmvwvvoav.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gfjrkpoxz.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/grvbooezh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gpnymtxqv.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gtkpixcti.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gdgxmkrwu.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gqquacgll.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/grqomcvlt.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gzliezbup.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gqjxnguux.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/ggedzkizm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gpwvefczs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/goclvuyut.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gjfhixswd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gpouzpmen.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gjmjpjyes.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gdvscpsvl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gftgjjdwj.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gckwvnydh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gznmiekqw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gqwqlqcvc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gytjdpzjr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gburewosh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gpyjmhvfd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gcyqtjckl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/ghmwjmctg.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gafuumtoz.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gfferneid.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gurcjrzth.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/ghkiwbqvn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gbshnjrod.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gvisdbsmn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gafhcigvd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/ggfstkgni.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gapdobpoc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/grsurumpc.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gnawjoyen.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/giabaqjvv.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/graygzlgd.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/ggwazejqy.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gdndaxjpr.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/goobgpiol.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gzichgghe.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/golofkmhj.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gmnzusoav.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gyfajccvs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gejtavpos.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/glmzelztb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gdyynocig.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gfxclrxes.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gjaznnxsg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gpxttqhwq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gmhtoomab.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gbkppewhg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gdiwrsenb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gkxncogzm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gcqcdumaz.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gxxbfhpvg.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gjoebwfmc.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/givkmnook.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gvlvkxnjb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gacnuiwaq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gabuecquo.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/giqikkykd.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gbactgmdl.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gcuwyqmlu.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gvavwktsm.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gznurnzoy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gmwjivejc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/gescfxfpc.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gtwmrqnbz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gamuwlogl.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gbiykfqvy.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gulbxseuc.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gvhhsaiow.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gunthtbqt.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gbnkdeykf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gssuthckx.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gelgixakh.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/grbjcervu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gowasixyw.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/greqcoagg.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gyxgcpeem.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gtukqyxrm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gcdtubpkf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/goxdypefo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gyqyishdu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gyinzsmje.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gmjlxbowg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gythlwsjv.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gtqrqaydt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gebzarlhz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gbhymxwrq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/grvtxphtv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gfgatffxw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gbypnczdl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gnphupowp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gxhirdsek.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/ghpgmrlhp.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gouksznrq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gupqdcfmd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gwndfceon.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gohwyalsg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gsfqdcegc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gjhtmzeig.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gjgxuskok.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gamnopdfx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gjngseyzw.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gihpwgwjc.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gxtppccsv.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gotnnjhgh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gyvoniplu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gywrztwit.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/grvlrosam.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/ggjbttfau.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gdxettayk.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gjwrdjbqz.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/giznrkxyo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/grptdznnu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gkwzyornk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gothjdqmq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gttzepfia.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gucsnbbhb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gjnekljvr.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gafttqgam.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gehwtesct.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gmovloevs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gwaableki.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/glxlwbppe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gnafgkhtn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/goyblkxsq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gpwedlbfs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/grrvuerco.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gxadfjkqd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gammwlwwz.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gmkppytrt.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gldezozex.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/govxdftku.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gaipmtvnr.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gnrjjuowv.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gpjgvtbis.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/giqfaprkh.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gwsyqgcrq.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/giovvolcd.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/giyukpazn.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gaoegommz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/guvnnuzeh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/ghratutxe.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gsufxbnnn.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqjboienf.sHtML


<!-- 参考信息 -->