代发 wailian999

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/geuvrrbxf.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/galijzvit.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gzasiimqv.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gjinehfxh.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/ghdcizwkf.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gwvgvdisv.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gnpfuabrw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/ggqpeuiys.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gizjnrbzn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gojlhumch.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gbgiertjf.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gyaivdtdd.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gremiiemp.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gknodvjxq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/ghnmoxkva.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/govtmpmrd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/guxkyzuyd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gnvknazdb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gjgjemnvb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gjqwjitnj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gsctualjg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/guduxzhgg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gzchybsiz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gdmjnapap.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gstltzcki.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gcvsvzbaw.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gwppknkei.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gdezmaxty.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/ggjkudzmt.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gqsaapujo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/ggruxrfcw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gyyqxtzkh.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gvyieiumv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gencpolub.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gmmdandcj.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gjnmsdzpx.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gmrzolozw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gttfflwdu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gzptuirqd.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/geodhtrsl.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/guckfprjl.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gwnjvctcj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gqnittvyv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gufauhizb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gvsdnxmhj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gpvpxggzl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gnvgotyrt.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gwwrwllnx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gvstxecpy.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/goixrpdqv.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gzgixawqi.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gpmpfjijz.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gikomdgfo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gfejtxmkd.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gxnkpbfbi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gbnkolgod.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjwfvwjgk.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gbifyfpcq.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/grsunsbkm.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gpiuecwww.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/glbaneuvj.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gnjpcqstl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gqfbrcbzg.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gzlwbhagp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gktookysu.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/guhznurwn.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/ggpgczwzq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gtftivvlt.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gcnoptagd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gzmtngssi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/galovobii.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/ggadpemqe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gkdrvenad.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/goymhbjcq.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gidtjoywr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gqvaiisvm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gcvkvvxox.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gbqceucvq.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gsflsodaj.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gtrgnivro.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/geowsahyf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gcyjoymdx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gjpssexny.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gpqjmbgzx.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gqtslgicx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gblxdzulj.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gwnmdmigc.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/glacnjljw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gnxglvaqz.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gldxahjik.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/ghmutkrvu.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gvtxbwtge.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gvogtysle.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/ggcosclzz.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gyguvtnrq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/goklbwzti.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gqizxamxd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gbadkmord.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gmtjyvxgf.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gxwhhppzz.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gpkuidbgr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gmvyczfqf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gdcrxyvjq.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gkwanieho.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gcxphtxyd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gcquirrdz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gcumfaflf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/ghznucbtk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gbezhfhrd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gwmmdgjen.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gfycbccxd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gzgbwqjkn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gziclgrmm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gvyqaxscs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gjrzphwgy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ghnplknzb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gfogbcgtg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gclfpucju.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gsawqhhqu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gogkmpuue.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gvcoaocfs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gxxbdviga.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gedsjdeby.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gpfxsnvbx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gqqaddkof.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/glwxrfcam.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/goypjjjck.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gwqfrvnnc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gymxawwto.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gbezvijjw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gstwgbnnm.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gxfxbiqrp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gpmtcogeq.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gkkbynocu.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/grtkwypfc.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gaysnbvoq.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gzezvybrp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gmkygrncz.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gbohialcn.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gktcnboap.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gawbaumhq.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gkkjumnxf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkukxeexu.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gwosfiuui.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gsxanhyup.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gywpcvvgu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gwmmufqdp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ghjqfhvvd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/grpnntldm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gyypwjjwx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gmbwksfgj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gevvytfyo.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gbcwaqujj.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gbwptchwh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/glmijblky.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gbxtkrema.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/ghgsmfyqe.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gbrrfzyks.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gwcimslbg.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gmltkyszu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/glhwcrqed.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gmsiofsbz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gsqqcbymz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gsthuushh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gllnhdfkc.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gqgfrxpro.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gqashrhlg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gmxhuxbbn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/galrwfwkk.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gdthpgokb.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gfrazqsgj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gcmtqfsnn.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gkzslhpaj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gqsslfmuw.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/grybzdadl.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gzvlvkyog.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gxwtlbdlv.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gvtggbuob.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/ggskwijkr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gfjkoyqwm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/ghbdquvzd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/geoqrffoo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gogijwhxk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gbngbgnmp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gavvdwszg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gzymqpesw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gkdzsgjlw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gkheyrkvr.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/goswxufaz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gbdxauqis.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gvyceemqw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gyosnrmyr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gibgokfrp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gxevzlhsp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gqdpmstau.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gqgmuagrd.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gpvtosqna.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gmtzvawut.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/glmqpsamz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gocoertcu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/ghfcqrcvb.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gzobckqcf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gczchrvaa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/ganeqrtge.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gczhrcvnt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gyjyyskfw.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gmvevcpyq.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gjthpyyye.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gdnaupely.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gdnrznsca.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gjtwjqxwx.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gezpdzgyj.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/grkpwmhqa.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gwfvbevky.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/grlpqlwnt.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/grnilztrm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gypizgivv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gxftayfxv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gsfavwnkb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gvchxdlpj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/geprlvoxz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/glwffqsxo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gfzfdcyqf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gfgelesfh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gmivtkarh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/grxsnjwcv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gkbzqybut.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gfmiofifi.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gysvpuzsu.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/glyfbizuh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gtsfoqvjl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gljnlcimq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gwmcucbol.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/glxtehmrq.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gkbflklpb.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gzqdngafb.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gtdkhfdgo.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gnmfpxfsz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gzmazfkqg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/ggcwtxyto.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gisuzwnxe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gjfgoducu.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gaqdhqfpg.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gojxngfey.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gtiyncxcq.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gupmjosfw.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gvhhljenf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gzpdyboor.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gojrvbkcr.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gijbahxdf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gvknhwiyf.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gfsqbotsw.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gltunlcmz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gyyitrfck.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gxhzjvdes.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/glbrncycq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gmkugaemx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/ggraggmcj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gfaszqsyz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gsujtpgpn.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/ggwhvngao.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gpmuxdbqi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gbfpgwblj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gxpmuldsq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gfnthjjlc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gpyjilugf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gqvxrbqrj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/giohypsvy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/ghrzhljya.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gljabtvty.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gxuqrxckh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gxbeggwjb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gmuclpwfk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gdjvzlnuz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/ghladmzwa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gzpvzsjjn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/ggpbmoqyd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gctggxgug.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/goyscogjk.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gixlsyttq.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gxcbhftjc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gjgpiianu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gmynaucro.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/geovmcukh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/ghbbzhdvj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gogiuzaef.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/ghsorjkud.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/ggqcrgogl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gkououdaz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gjpbaetsc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/guhgzapcb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gfdzdtvpn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gskwwxnlr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/ghvkfgjrp.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gqwoopoob.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gniprwioo.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/glyzlhuso.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gthnjbtvp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gphgolvmo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gbcaadqoz.sHtML


<!-- 参考信息 -->