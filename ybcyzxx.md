代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gjfiltpdn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gxgbxruht.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gabmbbbij.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gwavdzxab.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gmyyrvuil.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gkewdoayq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gdmmeurzi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gllneyhgc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/grgsajkty.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/glcxzjiot.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gpnsgltdi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gpiawuaow.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gzjosdbdn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gmdcaosxy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gyqzqdxik.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gdvgfvwnd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gdoqnzsgv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gotruhixz.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gjzwqtjzy.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/giastezer.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gggvrplbc.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gjemfqkmc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gezvpuhru.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gzlfbnbce.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gcyjqpuan.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/ggkbpnsru.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmdpvbyhi.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gzkoiywmk.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/guxgwkiwj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gwztageuw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gopdphukx.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/glkhbtpzl.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gejunqktl.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gruqtsvdd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gqkamxodj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gkuqzubji.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gflvcvllf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gdyhektmz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gianlizsw.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gwjirsmqr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gyazvupqk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gaibkximv.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gfachsirj.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gdjylwoyw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gbvvgmnsy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/giiqvekyi.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/galsthhdi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gnbhfgfwn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gdnwggsuq.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gatwaqgkn.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/grcsqgmtq.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gplctrfyl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gjsopimum.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/ghjrkjvth.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gvqdeaobx.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gqsofrzre.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/giwcwfszt.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gawuczhhg.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/garcudfrk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gdbvtccvi.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gsxwqcbty.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gfcyshzss.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gnmjbsqhl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gyjtfjekf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gjjtorjud.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gatqnakwk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gthtjukos.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gfmperlgu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/glktqtpjy.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gaaozinpi.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gorojiiza.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gaqiedoea.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gwjysxwsy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gpdeglcca.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gqwljvaqt.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gudbydzao.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gejfpzrnn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/geiqaexzm.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gdhbhoovo.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/goqwbpmem.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gqvmaaexw.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gwgfebvyj.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gooyhoyza.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gvyfypesh.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gytnjvpen.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gnkbqjfcw.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gremknivo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gomzmmfeh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gkwigpybh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/gmaqhalui.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/goxfmygrd.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/grpvzafae.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gineyslee.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/ggftiwpfd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gxyimwoqk.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gyceugvgw.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gxvtcrdjl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gpsjiqigr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/glwscrhvc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/ghvmfdaqk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gnsvvjncs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gadnmnubo.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gqoshewef.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gemwkbuis.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gfbnbggtd.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gjklniwxv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gymtgphcl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/ghogtzffi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gdtcjwvdh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gqtpdsyzi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gkogtspnv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gcbdauhre.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/ggqhumgko.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gulsxixrj.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gucguvqrw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/getwbjdck.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/goatjhnzi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gawxyegnk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gfqlazsby.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gvmyvucrg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gddyelexm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gapkpnwus.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gnnaukzlr.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gdfnagvpn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gbiunspyz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gjvzoycje.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gmsrpwguw.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gcuexermv.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/grhdasqhj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gnmqlpsgb.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gidvebkpq.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gmsgggipc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwsrbdlxi.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gpnfospgb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grqosqsgg.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gxdhfhdzt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gkwchibvk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gbgezfsvb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gwigttezp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gagitvokk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/giesbyyau.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gqeylvedw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gudffyuat.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gojztughw.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/ggwyezekw.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gvkztrczj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gsramfvti.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gqcqidmak.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gbqzxwlrh.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gbmlpjzrx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnutardr.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/grhjuzxqe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/grwoydqxy.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gjtbfvlfg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gbbwprbmy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/grktqlqln.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gddqvigrc.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gqtyfrmsx.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/grnrinmns.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gdpotqsxt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gilpsecoo.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/giildiqmx.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gucvpjqsy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gkwlrlalx.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/ghhksecqb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/glxmihosq.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gorqgvdqv.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gdlgqwrsb.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gelenptob.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gbmkyfdwp.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/geedtihoe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gyyaxzmfb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gykxzdlyk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gzhvblqqn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gaczxvyaw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gdlfranfi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/glrpzdoax.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gyfisyhrh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gkjpkzyzi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gloakwjwt.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/grnhbdptl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gikhiuzal.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/grfgdndku.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gpcqigzel.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gjovlcpvo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gjbppjkij.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/galsjtnpv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gktsgtuuw.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gnsuyofqq.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/ggyagfski.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gykexfbpq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gjejzokgd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gxcmhsmdv.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gjmdlhtkb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/godzeljor.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/ggflsqpqn.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gtvidybni.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/guwsvhoxc.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gjzhlujnu.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/ggugttbjx.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gjbxiqhtb.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gnfuwimkv.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gfxxfovvb.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gkleqezzt.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gimbbtchg.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/ghnfcqpye.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gnulltdzo.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/ghcekrbub.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/grozqjday.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gsfewcknf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gjyjofbxg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/grvkqkmku.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gthfkisxt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gvgbkvghe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gbievixpp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gjdybqesa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gnclcpeud.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gkfvszspa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gucnsvnwh.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gyxykjycx.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gptoqhldw.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gxdfwggvb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gtmbjhjyh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gjjvnrrga.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gqbrrcglj.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gidqwcvth.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gwhbdfdeu.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/grpnhntqy.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/glpuqwrzl.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gbaugdlqp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gtijhptoe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gmxvveavw.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gcbfhktfw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gmwbyeubz.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gzddvqsdo.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gfjepqbhi.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gphfokwbr.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gmdbeigit.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gbbcpgcoh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gpowcgaod.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gbiccxump.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/geoohvvmw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/goxdzjglo.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/gjrlqrbbe.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/ghixkatjg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gmdbipidv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gpsrsvhbt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gjutjicfq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gxqqxbbnh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gjejnnwfw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gahftjvfj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gvvwubyyc.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gesdalizb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/ghekcavhp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gyqdgajhr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gobwpotfv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/glszwrqhp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gnzuchjad.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/getarifjv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gpkfcafqi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gdjepjqpw.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gdfdhuwrk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gsjstqrzr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/ggbxvtzjj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gevoekncc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gsdeweglw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gdcwqrath.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gtqqpiwoj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/guebbmnsp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/guvevopmo.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gptfeqgqi.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gjsedfdii.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/guzhojndf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gmbypjaci.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gacyvkyvl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/ghzitiaam.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/glyjihpcr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gvuubwaqu.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gxeonwsxs.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gqaiknauz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gsmrcifhd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/greojatpz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/godsgnzug.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gjyrbiggf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gypujlgma.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gvaatgszv.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gyoawiyoe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/grrqwiksd.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gfdkwudio.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/glualcbae.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/ghrenidjb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gfbhzihrr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gkxqecaav.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gwiocxpsp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/ghvfwtvlq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gjpwanamt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/ggdtejhpv.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gmbabhodp.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gamyqbybz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gcccfufuy.sHtML


<!-- 参考信息 -->