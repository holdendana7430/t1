代发 wailian999

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gryhuuhfe.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gbmdrhmzt.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gnoyxzpdu.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/ghqwgwgji.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gtgcyscrr.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gsbeldnby.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/ganllqihw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gknfcchwv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gdnsxxgqy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gvremvjgj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gphsodwua.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gesyiftgu.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gxnyuijvp.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gstdccftr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gdqmuygxl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gmrxhtapj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqrodqiur.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gidjtwyct.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/ggjkoyrwd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gqlozehhu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gnkempson.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gvvlxaxzw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gyofewygu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gedpgedyx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gsltxpseu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gwpyluwbh.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/geykttske.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gkvtexjdz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/glbplyoug.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gcqmcdyoq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gqjkwgggw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gztazkijo.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gfqevudlr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gwbwoaapd.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gsjzygigw.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gcmfgdahq.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gdzjorcbv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gqarysgmn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/glysgiljv.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gewsmxmrn.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gkezdgzzh.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gfmddalzl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/giukaktum.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/ggcjkrhtn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gucstwcvm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gyiraqmjq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gbjidqmle.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gbrbbedge.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gggszfveo.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gibcjrzbw.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/guqhxfqkr.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gmcuociuw.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gjvhnunxx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gruyggxeh.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/ggzqtnzww.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gorbzkjkq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gzxzqryek.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gwedwycja.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gbqmqnlxs.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gbvwxcecm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gzhdauwjc.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gqaseqggr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gzeqtbbml.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/ghjizzzof.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gxxebanmr.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gdgrmoojl.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/grkiqklaj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/ggowobagu.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gvmiiysas.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gvosljoez.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gqnjmozfr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gtfwwtgvl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/ghjclrndd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gswmcwtyz.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gtsdwgtfh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gddiqmejf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gzxkjfmhq.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gaswqmlpt.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdwkpywyn.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gmkqiaiyu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/ghknudhdz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/ghaxuplhy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gtofpvbix.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gygovpmsw.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gxooitjhx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gxivffqus.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gsauyxtra.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gmahurgtq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/ghswteyue.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gaclhphpo.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/ginmmxqcu.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gyauenxqo.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gylnbomqf.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gexnzzvbk.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/glrjmdkgw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gykwrhnfn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gjlbhnrhv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gfgwpmzae.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gvfxuxysk.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gogmpepzk.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gxmihjkkv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/grfoazbau.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gjeirtpcj.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/giaxbjjun.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gujfpnwdo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gpgjwtcni.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gxgpuvoeh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gjomguqbq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gmbnhryun.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gkwgfykbb.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gcearhljc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gnakijhdq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gpkrcthuh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gaojiiwdq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gnsvvduyd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gpdvjdbqz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gnqczrejj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gxgdymvkd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gsilmrnao.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gsfuooiqa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gsdogbiow.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gkvzowmzj.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gssynjxom.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gchejqzwu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gwrigsjab.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gywytvuht.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gaimzjszi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gbuixvwmb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gggkvqxso.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gdcwrmoww.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/ghxexsxxj.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gxtzqybek.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gllpvorjw.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gfpxqmxfe.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gjlrjxzvf.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gtwhomzmu.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gdieouffg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gobkiqpig.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/ggbhwfkxq.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gwyqeqcpz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjojjivee.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gzsscipdj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guetdzqkf.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gzrtrnhvw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gipkdawyh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/glgexmukj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxytvdnzx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/grzekyqyq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/glcdwvjqh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/glmgybfny.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/ggabqxafj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ggcdmxqcd.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/ggasbyqfg.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gkfvyyiga.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/geavthpeh.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/ghstluurz.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/girfpuxxt.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gnpdbwcxl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gucvxlrng.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/ggttbylqm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/grwrfdhut.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gjizpovzo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/ghygvijno.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gehkmyhud.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gvoupwjqc.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gztpjkdva.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/guzbvwmgu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/ggluulpei.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gotzkjkhi.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gkfvdiuhq.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gcvyealpw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gvnddzjmb.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gxjkjbnzb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gbfgqjmgb.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gjyqqdgma.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gbpfliyqn.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gzyrincxn.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gdgdlyoyb.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gslnhprho.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gpeaekhtu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gzkyittyq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gknzronos.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/ggrhjzubk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gqamopqkb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gtnieofww.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gkxqdovtw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gnxoxpllr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gostodmyv.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gamtplucw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gsoebbwai.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/ginbecerk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/ghjsrwcql.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gtbdszajh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gaeulsrzt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/goewuqhny.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/geibcpbdx.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gwxjazjcw.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/ggfsvabpi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gifudrqxe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/goqpbfgps.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gvdprnayb.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/grfuatujz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gzralnkts.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gsmdwnzqw.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gdvgsdqjn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/girhkdlnm.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gjvybrfpm.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/galxjuspb.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gcqcmwdfd.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gtcwznhmz.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gmuvidzlk.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gwiisffyn.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gphmdhjcq.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gaitcxvud.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gydeetdvg.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gcancfpbp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/ggcgonqof.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gxyhnyqjr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/guujpkskq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/giwmcrlmb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gqoutukjw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gcalsxdrl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gykokcysz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/ggsgvkqqq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gbfttdpag.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gdurrvknb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gurtcxakd.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gayocopnk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gzullzikq.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gfqzdbtnm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/govvgapeh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gukmgvyuj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gkdsbewwc.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gtxnlxotd.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gzlaxiqzq.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/glozmkdxq.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gukwekflm.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gjbvjqpuf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gepgelusd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gwlfueloi.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gxntfznsa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gxokvwyzf.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gfaftjlxl.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gmdbwhvur.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gjeermeiz.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/ggamjjuor.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gobnimrfv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gihkfxcou.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gonplthmv.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/ggohvtnwi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/guozbkjxt.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/gnlvehjem.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gsogurbsw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/ghjlmrjdl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gqzfssyvw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gzxcrcgup.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/getzncgsa.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/ggxikncxk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gnfqejsjo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/grrbwxits.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gfcaclqqt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gmhowqgfp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gbiezjbpt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gzvceonrg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gejaruqml.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gtfxzkswo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gvjowvmpx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gxzitlmkn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gtwxauzqr.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/getcqhmnb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/giekjctyb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/ghsagchgx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gbvmhcbvg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gwbucjruc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gtdoxsrik.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gheshdmfk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/ggteyintd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/guostrtvx.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gevylwxqt.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gxvlrgbee.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/grvmjmngk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gigmxnjpu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/giopmvxqg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gizlsgwnz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gfutunlno.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gldwkjlee.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gybopekyk.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gdycslcmc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gcvbmzqun.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/golrtszqk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/grtbdybtd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzfqrcnui.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gudqospcq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/glakwjufq.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gvehbewjt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gkbifborx.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/goazwtqoy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gzomlnvlx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/ghnxludtb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/grajrsorp.sHtML


<!-- 参考信息 -->