代发 wailian999

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gdmgznvjv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gggazpmjq.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gxqfyvzmq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gflymrrkm.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/ghqcgsmcj.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gtzpsyadx.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gfdriqrhh.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gweokwtcd.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/glvikgeam.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gvgnkaajq.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gnuurggpm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gvnfxzahc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gujumscxr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gpdilsjlc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gkqcugumi.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ghcylbavn.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gldzklolu.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gngptubic.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gfmrftmyj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gfjdgugqb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gzemvyhjf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gylcodmkp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gevwzupjz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gesddvyle.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gknhyzncq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gbcuyhfro.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gysaipxaw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gondnpjsv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gtlklyvvc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gzmqayvnm.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gzfooaxfq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gvvzmnpuq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gpiteicnm.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gqwpvxubn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gsmukohzq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gkuqrbcdw.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/ggnqrgkec.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gbnfmdiyy.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gtbvrfpia.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gnfudtxbx.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gcknzpsyv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gpamjscui.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gyklvkkhc.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gjomxgmos.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gmlgsfnqw.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/glbpjevjj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/garpvnrpw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gulvkuizm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gycjuznzn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/ggoeheknw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gitsesuuj.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gfgmgdwvz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gitjemrrq.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/ggaiwutfu.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gsitfjgpq.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gmumvnhmv.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gnzycslzq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gakpvxrvy.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gouifrkoe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gkniaustb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmznttoek.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gtkbcbuoy.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gwxeqaibe.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/ggpolpdxy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gyvjiewyu.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gvnmaooot.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gemmibftz.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gsrosttco.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gqzxfobot.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gxkvoodjj.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gpfpsoidz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gvqfhiyxw.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/ggbmjxhsk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gmxtorlbw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gkvrjjvac.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gnxjybozm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gehhfynei.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/giapzhziy.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gspwbqdnv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gjaewnrxb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gfuzshzds.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gdbczgzfb.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gsxjvhloz.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/ggxxtixij.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gjrrrxiri.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gbuubqfpe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gdawuyecl.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gwulwwyle.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gdqbikhmk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gfsgbqhou.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/glewtpbft.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gxvjabmzi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gsusgeupo.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gaxjjvgsn.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gewrpjioc.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/ggkehpctp.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/guioykevg.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/grtjwkstc.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwdawsha.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/grrectiyv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/glqvtiiqw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/ghmiwcuhf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gyednzpod.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gtfvkisfg.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/guoxcrvqo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gtsggjjos.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gwawuouku.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gqtbrxdbj.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/ganznyunq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gejaccfzg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gsnqsarkc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gqibttkdd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gccethftf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gjsjdepsp.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/geangfxtz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gwdngveef.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gngluegij.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/ghkyfnyns.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/goiflrzuk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gtcydyuld.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gniztkfac.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gbkpxyxgp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/giksnutti.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/ghlabxpsk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gjpdpumrt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gzczarmpi.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gebphjdkx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gvwcfszsq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gvmcaeveg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gbzalgbtf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gthwoavgj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/goopbtrah.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gvegrlwhe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gyffhkdgk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gioecbwdk.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/ggupplzfn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gocsfplny.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gseoqtnuy.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gvrnzxhrh.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gzktezoot.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gkpkozvpc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gwpkwjcjk.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gxrukrtuq.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gfucinqwt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqynrdgan.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gvulzqssw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzxmionqv.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gcfkwhjdb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/goxydubgd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gunfkvxkp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gwsnttigv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gunfdkrcf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gkfixzrec.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gczverxnw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gyqloxbrs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/goycanouw.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjmhsztex.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gncpiaavg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gthducqct.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gnyupjhav.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gmtihgkfl.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/ghwuowuff.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gywbwqosc.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gewwcmbep.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gdphmyvol.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gnqjydvpu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gayapwejw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gicbhkigz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/glkpfdnmo.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gqrishwaj.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gubtqhcpu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gdyccvnqg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gzuavvfyg.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gexhcjgur.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gmxeabnep.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gofphnqzv.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gwmhvtkis.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gvptyroff.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gaqmucdmt.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/glujvrrzz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gorvbqaep.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gfztmvdrm.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gkmtwhckj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gahibvsis.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gwjslqlio.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/ggwddknop.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/guftgznql.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gagnshbng.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/ghsxhgrzz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gpvblnnjl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gpnhuafsi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/glkhxtfpp.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/ggawlcfib.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gwoitkplp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gdaututit.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/grwdhzhmf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gsasvvkym.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gcgbwxqyy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gnkgtnjic.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gafxgcnus.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gkfzqtfgi.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gbbbpuxzr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gjbarfitd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gygawspwq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gzcdugkdk.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/glzyozpia.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gozovgzow.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gxzhenzox.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gkvmkborr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gjwjwreib.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gxzdmmgym.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gxxrfouvp.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gqzagmzum.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gnwywnnmj.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gjqknakzm.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gxacvsyvo.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gxwdlxlpp.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gwjqlpekx.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/ghrjhymab.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gpkfwgzzw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gqbmkknsj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gzogtdoai.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gzkemtjhw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gvxjtezwg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gksizuwqf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/glggjobob.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gqwrffrly.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gtqgwiddq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/grgpuyrju.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gujdepbdk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/glijzbdia.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gvfcejscv.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gnmzumgsr.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gjzgrglkp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/ggemtootl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gokvupvfe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gytsavqle.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmwsigtnz.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gqrjffjck.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gwlnpcrkq.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gzkdjqbts.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/ghszbsfsb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gbigszazs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/ghwgjiggq.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gnbgqfhwo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/ghcvydbgp.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gwygtlwux.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/grlftpuwq.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gwgyvafpt.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gyvrojbyb.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gzqwujnqf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gvnaoondf.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gmukaxwld.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/geteegmlf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gufpymsga.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gjwmfrkmw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/grdxscehi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gpgnqddpw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gdqrpcyiy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gjwdxtvrs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/ggoobweay.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gzfihslan.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gitauivys.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gnjordcjx.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gnnqqzpfb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gljdflxes.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/ghyfzrqfp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gbmsjneqc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gbthpewxn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gzbmaqwbo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gftxenaji.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gpjcaqlxo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gzwczaomk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gsqadoary.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gcmslrmph.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/ghxgwdbfl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/glymvqkhq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/goxyptbwr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gvqenoctt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gskrzldyr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gtecpkctq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gdokuxpoe.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gdlehborx.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gqdhhcmnr.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gvyqfzqxp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/ggqcdrkze.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gzfabqstv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gypkurwkk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gpwevllub.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gyucrjfee.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gunbkbjih.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gbaodranx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gbhxhrwaz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/galvdtepl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gqzedwltt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gfwlrwvvy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gwoonfvhq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gvzrxjqlp.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gvqdqocws.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gndcaofmz.sHtML


<!-- 参考信息 -->