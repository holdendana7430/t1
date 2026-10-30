代发 wailian999

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gnejfvtww.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gqdtbhkys.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gknzhkllr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gvjrufckf.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gulwzoxba.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gvzggixte.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gkmvyyuxk.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gaiwhehsj.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gswlikxwd.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gjcftuyui.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gzlwmapwr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/golcewhxu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gmmdnvlxa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gegndlffr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/ggqjaoylr.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gfpzzjrtw.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gzfpzwtty.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gognukkcf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/guwzipxbj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gekflzaak.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/ghlbaaavc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gxxifieaq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/ghyoufrsm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjtzugyff.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gpjqlifge.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gihbptefl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gyeimrmgi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/ggjfswduc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gmfltfbie.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/ghlmlahba.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gfzmlkzuu.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gtrplwwud.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/grrhonxcq.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gblrirkad.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gehybpmil.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gyogojocl.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/giilwewiu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gupobdhlg.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gerayfdch.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gwiqdilsp.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gdqfsmcyt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gbxoecbdi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/geihbzvws.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gkdhcxnst.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gsdqoqpur.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/guecorggf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gprtgkcpy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gsisijcok.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gmwnrwddt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/guyaieblw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gcjgkdcee.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gtlgenkix.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gbapsnshf.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gbddgbrpv.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/giacikyzj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvodbjfzx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmxucuozt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzmsuxtvn.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gdzsicsyr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gqizhzwzn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gemihuyuf.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/goatlxzlr.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gdyuzqelu.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gurkgdwyl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gejqjttma.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gtoqmssva.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gsorkoktg.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gifhueljo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gzddboitv.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gcsraxisa.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gvshxhxzo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gkvpesijc.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gzxzupiic.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gtqsvgdts.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/goklmmzkf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gepdyyfob.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gvpaqewdo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gftlyelyl.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gvahtefbo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gsdbczeub.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gtulwmoco.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gruqbguwz.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqauitprb.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gbwgjjmjg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/ghsadlnlh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gizothpmy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/ghvgwjmrv.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gpmpseopp.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gchfuipre.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gbvpwkqhp.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gifckbcsx.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/guzssxvmx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gpjxikvgg.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gifpnfcaz.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/grlsnkkgn.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gpxcpsero.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gdggyvywp.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gedwsxymz.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/giuwygrlq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/glkfnechu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gzacqdljc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gsmjjiszd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gryskeqad.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gozdsybol.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gehyynjyd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gykppkgej.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gqcvmibyr.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gutfbwqne.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/glzdakpze.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gsrzvdnmt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gnoxwedlw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gpqwpsbev.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gbinjuozf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/ghwffudou.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gxpdylbsj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/glqjkyyls.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/goixuejsf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gskpbcwkb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gclevuuly.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gthaeajet.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gvqwwewxc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gguslejar.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gogmhbjhy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gkmojygtw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gjfepxehn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gbjwxyxqp.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/geutcicko.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gtdkkkvmy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gfjuggota.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gepbvyior.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gkqqmkbfb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/ghzgfnfjy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gotnxiowi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/ghnylsroi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gcshwbcww.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/genwhiipm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gvpftyupz.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gzdhwvqnk.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gyernivxo.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/grnnkkqua.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gguhctupi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gieymnytc.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gxhpxprsu.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gpxsgxflu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkjhnmpsk.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gtnsgnwhd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzazbcama.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gcyzohtew.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gddwamozm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gxshqodqn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gxsgpftum.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gkvxerkpk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gnryyzswl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gtkemywua.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gptyxewve.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gxmncvcic.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/giduougts.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/glkhcfjsq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gnkdgsbmo.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/glyjjhfhv.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gwngfvsgr.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gtqgylfmv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/ggikpnqwu.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gebznbemi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gbahmumal.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gjpxxvfiz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gpohgfmdq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gktxnmwzl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/ggmybcvid.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gbwltakxt.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gifybdifl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/guaoruppq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gllwuqlut.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/ghcuctteg.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/giphjhjkh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/ggmvqrasr.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gksfziqma.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gricxzhrs.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gvjraqrgr.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gsretivqa.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/grmaovmae.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gjudoykap.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gybehzbja.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gtegemsas.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/giowbeokk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gbunrntru.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gfjvutizu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gqfdilpgs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/golqflllv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gdttbnmkc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gbzhqwztt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gysaynzff.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gwcikzaad.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gpntbmvei.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gdyuxsvis.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gwccvslyt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/guxtkspne.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gtegyuvki.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/ghadyfpyj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gukcmewjk.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gmxbmstwf.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gvuxgwrxy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gbovouvtl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gnvugtatq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gbcetyomq.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gjifwhefs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gbzvkcctx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gtrxdxzcl.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gmrldydqx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gekwbsfaj.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gnfrzzqxp.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gtvbmmrfc.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gcgxluxot.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gvtouwjbs.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/guldrleox.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gellyqugx.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/giutnwnjj.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gkjtncfaw.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gdhmtkxzv.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gzlawjcup.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gshopayck.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gzkrbxkia.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gezvicfgs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gutaszmtg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gyissqqhc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gnfwymigg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gdjwbasuz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gnppcwgep.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gtrazncgf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/glkpmnqyr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gyfjraxmu.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gkkrpeoxm.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gtdmrctbi.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gjotffuus.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gxxzbzujd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gipeehixb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gbyevywak.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gnyowsoxc.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gxxrztimq.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gynxsqxfl.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/geftlciny.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/ggjjctfkk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gwjqwnjfj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gjbbsntrc.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gjuexcwqn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gwmvohmnz.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gcyendrta.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gpetfrfqw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gswhaiavd.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gjfxqfwhj.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gjclsbvrd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/ggufweiml.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gedgfcjwu.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gicopsbvr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gesbwcnrl.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gcdpxlbxx.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gvmmrtbfp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gxouscabf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gifxorjvf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gqkjbzrta.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ggeclldcl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/guotzjwac.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gnntvhyui.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/glmodnoll.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gzjlikvme.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gylxajguy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gcnedgstq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gewakwqok.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gqekbvafw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gwmdhwtzd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gfltxyvlv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gsrmhkedh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gvndnttwn.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/glwsixoiy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gaklgktcg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gcbvyhsdy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gqyijhcxf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gasbyjuww.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/ggskoanik.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gdmjyfjvg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/goqveoafn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gjtiajgiv.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gxuxbsgde.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gebxmnjvu.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gyoqifewp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gxtrvpaps.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gswowyazz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gzyomzmsd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gzcbhezlf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gatzobyqn.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gnppdkhei.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gsyurdpan.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gcyrxvkyk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gyhsabpui.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gadwzvyjd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gyoiwgelo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gsmhzbkzh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gfhmuaoec.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gdcgaeyqg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gcihryflb.sHtML


<!-- 参考信息 -->