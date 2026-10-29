代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gvuqlghdt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gmvwjgpzh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gdipibygc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gstzchncp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gghsabbcg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gvtapybtz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmzfpyvsq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/geooqcsqh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gdugsxctt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gjfuoqsov.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gaezgqpuq.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gplxtgsxz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gansrjwpw.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gdydeenby.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/goojaqzoe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gzwbjzwmx.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gagzqavsg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gsjjffrri.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gflykbwzo.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gepwqgvet.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gteipaldi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gvjmsnpls.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gdwqzzkuf.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gixinqdht.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gsiqmcbwv.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gfykdlzin.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlfrerpc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/guveljvgk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gypbshwch.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gsxquxvhy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gkphdwbkx.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/glxecysrf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gmyzgbmdr.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gxnfhqlqm.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gkepmnabt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gutpsijop.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvtvmuvls.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gpkunnwnx.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gamgohscp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/ggnaggyjp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdyusxghz.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gcfrmzqtk.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gqntrbrni.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gsylxwhar.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/ggehsztnw.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/garjlcbrg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/geiayqdzb.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gpixsvyhf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gacbgyqdd.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gggnkcfqn.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gyjmjlvby.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/ghabxsyng.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gnruxyddg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/geigxgrzm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gkdotahhl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gplnyyzzi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gdytajqao.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gtosyfeze.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gxsqusoxa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gobsyosna.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gtmocqftc.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gflfgsqbu.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gnofzdjhz.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/ghxbtvgpg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gvopbpyno.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gipvxgwhg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gcngfbbbz.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gktwjhlpj.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gzyruuogn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gfxyjocsa.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gmhsnfxxh.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/grasgmtxo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gnvscobux.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gpypitupu.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gvvtrdmrw.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdqmfiows.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ghndqtmze.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/glmxnnpmv.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gpswrvgvy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gqfilwtok.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gtlcsmvky.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/grpdqglel.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gndowkyyc.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gzyanujfd.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/geamijdsd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gunwylpgs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gtfgzsquh.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gdqqlmfpu.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gobekelev.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gvmtxmtcu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/ghhuyttqs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gjjrghylv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gryopqgld.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gdypaymdu.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gidfraqxk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gitevmwmy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gzpouqgbh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gxjneaojc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gwfbdkvpo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gtcfkafcj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gowxykicp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/guowurumo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/giprekcdx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/giwbotdjq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gztkmssye.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gubrgwkkq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/glpvxzewg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/giusfujwm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/grhkddsdu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gxdrcnqqk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gsqqsvnom.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gilprgiww.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gbyepwzrd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gqqnmmyha.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gnanhzpux.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gfnxrutny.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gjolmhpyc.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/givtviggk.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gazjfwiwa.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gqheavevk.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gfzwbeswv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/glkgeuahm.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/grujzjtww.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gbvzunozq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmulvxefz.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/geqnrdjzr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giahojqqn.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/ggnizipsw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gfbidkkcc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/guzofecae.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gwiuiaqfh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gxindgrte.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gnpoaylmk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gpadabrdh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gjhnuybtp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gdnoqzeoi.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gscknmvzb.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gpjgtzusn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gdriyadtc.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gbacxtouc.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gfpxrqmrd.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gitctpoto.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/ghzygfoak.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gwmcdrlat.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gbnvxmnla.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gdoyivzlw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gxrzgcrtx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/grjohwgho.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gzevnzxya.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/guenikqro.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gqebdtfjs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gjalziojf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gylgctihk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gxkbqcxyz.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/ghehsbhlv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/glttwniho.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gipmblrpq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/ghpyozwjh.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gmoaofwcx.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gysiwenrc.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gmyjulzhs.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gffzjghxc.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/ghkoztwck.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gmzvloawc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gddjjeeud.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gaxksuytr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gaxoeryxv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gtkawrlur.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gzikxnlek.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gyhfmyvyo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gqcjsjblu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gdjmebaft.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gbpubwlbd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gstjcmvrw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gohrkdmvt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gryzlksih.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gvstudupf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gnrexryht.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gwepwsnom.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gqbvnrmey.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gxmofolaw.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gcflutkje.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gxgbggccj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gkebkwihi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gmpzmevrt.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gouphyrht.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gflkvzknr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gzigwqwkb.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gwcrzmqte.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gwtvdqjhr.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/guxktcqtw.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gqgvzaajj.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/guzhcwrsu.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gssejmyeg.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gncvawski.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gtfdidulh.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gtpjukkmu.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gdoxxtese.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gogkggzgw.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gpfwmpjgh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gkwirvgru.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gpgpkfwrb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gljfilqza.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gebbnxjge.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gbcmbzhwm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gbdqtgebp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gghhpmceg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gvlzcansf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gigkjhtli.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/glitxcbpn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gtkxwuunl.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gclpltwjf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gecactcrj.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gziziorkc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gzrhstomq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gekbqkurs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gpavjzkdr.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gwyyenqmv.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/ghxxgzhlu.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gwscbxoxi.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/getdwlkls.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gyzwkvnuv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gqtszbksk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gbfihypmy.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gpzmrtnrx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gaexlfttn.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gqydpnnax.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gtukarhwx.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gwdcfevdv.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gapfrmgkc.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gjuwpcrjb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gvewcwoks.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gmnxxptai.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gojaextth.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/greqavqey.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gzpgyluam.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gmhvwbewj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gvxkdkvmc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gczdypymt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gsxevdaky.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/glxvlicst.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gqxrdxcly.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/glzicxjyq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gsdkgutso.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gawcsrpmo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gcwupbdzs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gclicnjnx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gyopoyajv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvbcfnzlp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gvlymncvg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gwrpftnus.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gdzzvfeob.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gfqpadwgq.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gyakitqyr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gvxjtsrzt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gyobbwxca.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gtivgmnnm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gmlvktgax.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gnilluyxd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gvrujonea.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/ggkzxnudb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gxtcxhyjb.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/guorcxfcw.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/ggtmrhxuw.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gydwtcruk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gytlzmuzg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gjkqvbixj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gvwljpxfp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gagqwixdj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/ggtazivsj.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gtbbstbpd.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gxcvtwsuo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gvqjderia.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gbbnlhnkm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gluacabno.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gywdwbqhc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gctmnrkeq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gdbcqmysz.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gwqhwdmnq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gupvrnean.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/ghhmyrleb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gxxtojakz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gkyzzvrmo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gvpmomqcq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gtjcxulul.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/ggclzxfsw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gshasiqbx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gszwajdmg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gsefcoatc.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gpwrfyefe.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gvinxwopz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gyeawqbxz.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gsjsmcniu.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gominywup.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gtbaclobd.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/glkqhgjra.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gnmtzvktp.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gjeekrxel.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gjspsugib.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gnatpshri.sHtML


<!-- 参考信息 -->