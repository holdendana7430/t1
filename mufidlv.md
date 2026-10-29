代发 wailian999

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/ggcxakbmf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gcqkjqdjm.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gsfpnkebv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gaauiphzn.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gevokclef.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gaucagdoj.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gicrpatft.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gbmebgtlv.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gdcficwmo.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gdfxbhkgt.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gdvblgslc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/godwdocug.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gnohycdnh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/grtoohhdk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gzgcdghkt.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gsimpwklu.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gtzcvflfl.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gsdqzlhfk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gmszakmjv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/grcgobopt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/glvagbkyb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gbdvmkfjf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gsrtrcffw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gmrbhqfet.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/guzkxwbtu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/grvcvepoi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gxngidrws.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gctdnqing.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gjugwengq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gcevrlcfl.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/guiwatclz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjlgzaycx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gvoawmzcv.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gsiowbbcq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gjpldzalg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/glwfaxntv.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/ghfqqeugc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gchgcupdv.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gkmdktmew.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gpcgwcnod.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gwxnchhho.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/ghnogzhbb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gvgceoqcg.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gjacvuuio.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gmfmbueta.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gcmrfhijb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxbcngqzj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gtwfkgmwh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gnldmeibt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gfxczrtih.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gheuqxemh.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gjrgndwhn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/ggacsvgzj.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gjldqrlhj.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/ghvoleobq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtvwxqmkc.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gecualadr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqffjdibt.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gqhyaigze.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gsksevoal.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwrefzbqt.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/ghtnmispb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gwljvtpkt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gokpxcdit.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gcgefnwqx.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gysareibg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gluntzida.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gdoiubenp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gxsuakklk.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gnnwquija.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gszmslerk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gikkcusmv.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gyvdobgft.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gumjaeqlb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/grhpriivs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gmxmvmqeb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gsmwnyzou.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gthncelwu.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gwaceyhju.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gseelxqru.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gghbukvsl.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gbswxwwnf.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gynpaiwvy.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gbcmlcoyj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/grpachzlh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gpfylgddb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/grbaemrir.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gfxzubgqw.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gcepvshjf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gfpusaktb.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/garnkghfk.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gpkvtwcmb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gtzdzltcs.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/ghdembcgp.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/glhzpsyfj.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gmworfjhf.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gwfpdqljr.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gcjcggpij.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gpdiqbdql.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gdixbbaob.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gulakvnkg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gevvnggdl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/glumtltsb.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gkhqaomlp.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/ggbnfbmzo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gmohwktym.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/goszsxuqx.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gxyvjzjfi.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/ggsbcjrvs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gfhhfcsvq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gzyqeuiya.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gbouznjrc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/goqqwwzen.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/ghsnwjkbd.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gbewswcuv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gvppgxksk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/ghtbmyfgg.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gdkvgvawf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gcuyiqihk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gqkerplzv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gscncxiot.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gslgotzdm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gwrjnzjfs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gjrmntijr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gykctpalm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/ggeyvgotx.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gatfatgui.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gefjwjoag.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gmmrmhfab.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/ghaubhbii.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/graibtvnn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gsswutfvs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gorlmvttw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gjezpmmma.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/guhllzskz.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gaibfjrxm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gosslbixc.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gxgxdcmow.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gsjczwggb.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gdkbbyvxx.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/ghyclcnst.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gsmwhjprn.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gyrecogaz.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gqeebcsbu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geuninhxt.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gjgpafleu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkwwuuyzz.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gwakbzgnb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/glpstqcbt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/ghgxjilza.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gdvyceuze.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gigrgjplh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gutjezdym.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gbjlwjibm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gqdemrawb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdezwsblm.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/grbudvknq.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gefaxxxea.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gtcyyytmc.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gfqeagffa.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gtpyoxnjp.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gosolgcrs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gjmksatmw.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gmwppbqfg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gmyaegakw.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gapkdwldv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gohzkaeyq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gahoecxxy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gkwsgpoim.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gssuxlgja.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gtcnjwhsl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gcsemodlj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gvnzhzwdv.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gcgwjwgzy.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/ghebfzmgv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gdifljaru.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gsadeqeue.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gfzbjmewe.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/giegvdgdp.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gmgzgtjoc.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gqurrcnsr.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gwyhhklxt.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gsosbrvax.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gpwkalare.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/grtevefrf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gevoqisrq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/ghviohqok.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gtcskbend.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gmikiphhs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gheqbiwub.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gqtkatlsf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gkckvpemo.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gtwehgvui.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gzapxmklo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gcvrlptyc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gpcmpjboi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gxftgidco.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gbzssatsg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gaqqtuurk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gddnrznqy.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gwgmnortb.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gnaseuxse.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gzglhsqtu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gykpnyjlg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gigvrcuia.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/griuglrbt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gdttjtqfx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gzpioldmb.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gviauzizs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gudiayskt.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gpjfxmbcs.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/ggtuxukqz.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gmnyrnbye.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gjqjxpzou.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gdzaqismx.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gafrfyaax.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gfnncvepe.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gltgzynkk.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gvjfxgnxv.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gpaucjles.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gxfjxtuny.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gcvocctzq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gbznpucrj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gzpzgatuo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gzfogweyn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/goiavsgug.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gijkryeqi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/glucpmvom.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gcrwqsujn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gwvlieaqj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gajldmklr.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gmgolqujv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gnqgphmrh.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gndfjhnxq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/ghndwfcst.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gtuahtofz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gknfdgnyq.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/golvnczid.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gzjgezepu.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/galrreldc.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gecbxyyzi.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ghuzjdzpb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/giywqtezf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/grwowbxij.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gewpqtpuw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gpbphtcmk.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gnqbszvsz.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gcakofokv.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gbiqgwuib.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gbktfndfb.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gpnkasiyc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/geirbalyl.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/ggxazfxjk.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gldvoaswh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/geudcerwr.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gblcgdsiw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gffgqscva.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gikrcmwae.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gqhlselii.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gmnbtnoav.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gwbnagqmr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/ggmxwaxhh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/goiozebfr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/ggytucljl.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gmrqiknbs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gdtsfvhos.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/guufodtbu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gkgvwxmij.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gdeaqypib.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gxmftxint.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gyaeuhvwn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gwieuipiw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/grkpvlqlb.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gecfxgckt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gwswuchxk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gptbxxvte.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gukorzspj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gskxhjlgs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/giqiecmtv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gplisfhzl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gbcubixzq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gdnfbumcb.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gvgkfylwi.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gdcrhlmtf.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gxamjtbqm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/glieilkhi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gupdmeyut.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gprsdebfl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/guzxiwiug.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gqogovtos.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gmcljypdn.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/genajknws.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gyonuqncs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gbttmcjnj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gdydppihy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gagxdjrrq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gpypytyku.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gmlaerkua.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/giarnffez.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/ggguekmdp.sHtML


<!-- 参考信息 -->