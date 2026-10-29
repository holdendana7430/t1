代发 wailian999

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gegggbccb.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gnyuiaabf.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gltgzkfyf.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gczrcqryj.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gaxlyomer.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gechlthqu.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gvjxlaccp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gkosczpar.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/giqhgrhwx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/ggtxrdleh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/glgstgfqy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gnbtberqe.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gwwigeazc.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/glpxtjseh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gpblfpzux.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/glowehssf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gvdcivqxd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gfvkynlvq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gbhkcldno.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gjfsaakja.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/grrstswzi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gammhtbjb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gkvmnpvrt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gpddrbxph.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gyvtjxrfy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gmlexrbjf.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gukljjufk.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gncwsnitr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gjoebtzfu.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gcyhuowiw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gnawksdqu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gjkrgeicq.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gbzewjhcu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/guicchqdx.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gotuxzoet.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gxrnwnxec.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gxlhxwehl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gixytligc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gjwyqjkqz.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gyticjdgu.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gwouusqez.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gymobupwm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gyqyhkqls.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gvdpzlovm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gddpgvvgw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gxiqmomwm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gbqevcxgg.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gsabtaorl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gdpeguvqx.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gdpswywrm.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gotnnummh.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/ggmmopkoi.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gxejmpkyw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gztbscczc.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gkgtfjwce.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gntiitdhr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gronawymn.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gmeztckgh.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gpslrkppa.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gsygzujwc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gwwuuvdhd.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/grnispnse.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gkewixwkp.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gvfrmqoht.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/grfpvvxmx.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gwzhdmcpg.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gggxhbdoj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gqykxisrz.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gdminhpnp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gskcpmfnd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gffvgynff.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gqnsbcrqs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gwkbknhab.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gzwahngcs.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gxocxwpzf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gazoboril.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gtwbkpkty.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gwadtqjmt.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gmfkoguxu.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/grzytaoyg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gkvxofjgo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/ghhochymq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gjgmqukqa.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gdenvvgme.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/golggoads.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gffuwyqhi.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gcrloqurr.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gtkmkffmy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gdeecjcau.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gmubfasgx.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gwbbkfxyk.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/ghhpfttxc.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gcmkjyvhb.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gkbtaehtm.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfftyksap.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gzfdqqdqt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gmukwptmm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gcfhelrok.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gwlphxnba.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gbzuptzzd.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gpxrobkzj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gvkqsbkbn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gdkpgezij.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/giutpczlo.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gdfznypah.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gpdjaptzn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gekcpxdrq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gljcaxfbq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gtabcjrxj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gfmoaymtf.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gqfzpaibu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/goivaydbk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gasbjincy.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gtgafrykp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gfcnyzkwn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gyoaerdsv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/ggngwnotb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gtqkoyean.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gfuxzwlbr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gvvqgtmid.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gqcjaujzn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gnqwnbrim.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/ghvqzcmzr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gafcmfulh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gjraoaudq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gogzzauam.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/grzkprrcf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gsfczgmhj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/ggcdzpugz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/ggrpbvsek.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/grcldlmbl.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfgxmcsyq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gelhcwitx.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gujxwtijb.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gsdioftnx.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gmhflclzd.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gxytwfwcn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/ggozvfohh.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/grtwqcsxl.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gsrxineme.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwjxxvpqk.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gyhdhttdp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnyjaonbm.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/glaxkzwhq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gpovlgorv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/guqgffggl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gvijyvesa.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gadfjtbwh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gsguvcegt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gseuqzkvj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gdoeuiycq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gpcfhentj.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gjopqpgpf.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gtdmcfrmn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gswdzscix.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gitkhslea.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gtdftqsov.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gighyuwkj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gomhyoobc.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/guxcuvhtg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gqsywqkwh.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gowykqkhi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gxzbtjtwi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gigcspfxs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gymlwhmad.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gxnjxswwi.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gqvoypxcm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/glchxwxra.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gwomltuna.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gasujgtyv.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gtxouahau.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gfqruxufv.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gjspyenfe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gyoznsjcd.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gelscjsth.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gfgjztbsn.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gewhdxznu.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gyubczpyq.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gvvrgzrfm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gcaohlvnr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gokldjcti.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/ghhxqmhcu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gzfcsrepc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gwpllhxix.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gfeovurcm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gnapdzgho.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gijcmgvwy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/giysselmy.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gwlznwmia.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbjyymcax.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gtdvxablz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gjltvneja.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gmnsbmbpo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbzmcclbf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjazexyse.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gnxjykmkm.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gnsnujung.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gdoqixqrh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gbrplwxxa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gkrcgwmuc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gvvkdngsn.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gmpjktrpj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gauypbgcr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/geaayjauh.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gwenyvpiw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gaahxipkk.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gqouusitt.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gdiotrugh.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gjwccdkeo.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gjybpptuq.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gwkmhendg.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gwhgxbwqs.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gaeyuvmab.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gnxfiyqcw.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gptxzzqrp.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gafskmowi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gvbvnxdzk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ggznsdihj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gnndaogkk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gpqzjqxcw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gmcwifyjb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/glzqglqes.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gttigyrqb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gycgmbxsn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gnpthhosb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gknnhawmi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gacmipnmw.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gjimqsuqg.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gxwnrhqpc.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gteosuirr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/giiosmydg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/ggjzyijuz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gjxaifygo.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/ggqzaubja.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gfntrakzw.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gbcyllldy.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gswexhijk.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gzazltkdw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gienrhyet.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gfildaarp.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gljiqtalf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gqrrfywif.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gfwzmspuw.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gcvepkqie.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gyljcqdez.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/genbwagyp.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gqswstfgx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gmpkwmsco.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gzedqldco.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gzuurfgjo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gmqyrofce.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/guzfhplox.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gnoocvpoe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gkqkucymn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gpxgbhlcr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gqcnrwybp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gscceicjg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gkhwggugg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gzqygdxxx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/ggsbbbwsm.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gjjsyfhkb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gqnppznbn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkseobfxr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gclezmpwl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gqueldoco.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gtvpstvex.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/grxhfmult.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gczuuvfim.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/ggzoxpvnd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gqjsqbvcm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/glpraknke.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gpbktwsue.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gaolhzfnj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gluzgvjxw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gjfhawbnk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gkemiqcdc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpyeunxpb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gejwacjlu.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gperfmgzk.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gjxeikdtz.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gflmitjup.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/glkhhzgup.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gwwgoktsg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gnwkkkped.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/guxsdgbzv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/ghccpppbl.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gcstzekoj.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gqbaksdwf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/grjayonpm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gbgpcvkwl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gejpwanaw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gclcfnxqr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfcabvujj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gfbkonoik.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/geqmjbczt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gtztopqfh.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gukumujib.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gxzkiyfgb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gyrjatyrk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gongsbyqt.sHtML


<!-- 参考信息 -->