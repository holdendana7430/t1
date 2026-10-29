代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gttqrwjdn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/grfaagkwv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gpxisgpmd.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gfjpyvsfa.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gbonvnztn.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gvdcqucry.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gfpljkznf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gdfctztzn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/genzmsvxz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/goausdfpq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/guhbcxuyk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gwuwuhjaz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gdltdvkuy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gpropfmkg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/grgauzbqb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gbbsxtnzy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gxjtkjiaa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gczlqmssk.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gjkeutjmx.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gvcsyarbs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gsjnuxqky.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gwfxfxqux.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gxceplgzp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gldmjafet.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/guzcrrwcr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gyqofqukw.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/getglhiqt.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gbrolekbt.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gsxpcpijk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gnbccxldb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gzbbfuhtm.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/ghwcdjtsw.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/ghxeiewvt.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gesblnrfx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtezojfxm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gtxolrpvc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/ggswxlnsy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gnhaokpgj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gmajdbevz.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gczndrqtm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gvcjxfsxo.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gpberdojm.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gjwlkvwbc.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gylfufcoh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gscfvoalf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gvjnpebxa.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gqjgouahy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gpxcpgqil.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzirregvp.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/grdxsytok.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gjwumqsoo.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gfznvrwqc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/ghpmvbyjn.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gvcyhwruw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gpcbrksjg.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gdbteunur.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gbzghkzqn.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gdhzsitqb.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/giqcvjfyk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gscowzpxg.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gzkobgxmh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gjbifxyns.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gtqtnvlqf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gilcgyrib.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gfigvxcxv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gpbtitakp.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gmwiujsov.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gqtkebppc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gqxchvzfg.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/ghywjclyc.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gowfpdmbp.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/guwathvbn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gearezkkz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gcqtslkks.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gyfxihuvr.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gtiqaxzho.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gnybgvatj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gmakoosac.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gfhxapkbs.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/geznngnrd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gaunyaown.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gviluhoqb.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gfkpulrwy.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/glnkhryic.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gwmtvcbgz.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/ghxgzymyk.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/grcmlrosk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gyqdprajo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gefvdpqqm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/ghagzweqm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/guipiwqbm.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gjefdwqqv.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gkxugnpod.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gqwlbchbj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gkbcfhemr.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gzhqngsys.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gcahzlqox.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gukyjoykt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gbbktjaue.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqdoodqb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/ghvcewnsw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gsxljvaev.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gxwfgqqbp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gpmrfecfg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gocecsxyr.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gkmconrgx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gekhvqapf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gvgnzynjv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/godxvqqow.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gpdlqpvbg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gtwqvrqft.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gfcxevenx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gmjxgdaye.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gzigatybi.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gqmtkfgdu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gqfxzbwyg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gmzjdazno.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gnyqykgst.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gnwdpgcwm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghwrrftlj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gtryncics.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/grwfinmgf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gxqndlcra.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gnjycdyay.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gdokpftvq.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gpqtlxcnf.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gbkgusdao.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gvzsmcjvr.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/grxfrhaox.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gutzlajoq.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gsxzanaae.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gsvkutdfw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkplilpff.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/geztgjbmb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnadbzjck.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gbgydkfdq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/glhkhigos.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gwtqizllh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gqvjzmxnb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gggmfhzsa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gthvfcsgh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/govxocwrg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gqtmclouh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/ggfnzwmrz.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gjvmabkqf.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gqgcjzdmj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gfkycsbtv.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gniddvbxj.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gjdeufzew.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gwntioqpw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gkcevlbui.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/glftbudxe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/glpxnwcaj.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gzmnwkffg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gchyytfib.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gjetvwsnr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gnybnogeo.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gyodshxln.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gvlkczizv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gtlbmbvtz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/giynljiro.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gjjzvnytw.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gwneycrag.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gquftdein.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/glduyjkgf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gmtotpejr.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gisawsgpi.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/glyvvowoa.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gagmlfabe.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gdznpolzx.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gwffreysg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/glzdmvlgf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gxyfmnspl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gtagqjygo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/glqsmnpfb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gfgeojwxu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/ghvhculup.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gyvpgenqh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gfpubkcxg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/ghmzcvtjy.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gbcmbbkqn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/grczququo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/grcufqehd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gxbijotif.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gmquzgyfl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gyerseghm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/ggwdvztja.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/ggslqvlqy.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/grjezkuyh.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/ggyptaeps.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/ggwaphinj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gtbaxzhne.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/guufxzfov.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/guomavenn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gacvaawix.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gqwyvcitj.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gnjzbxkhi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gdroxiynn.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/goozwtdlp.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gfaeizbjx.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gbovwzokv.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gntzqelyc.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gsnhvvbei.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gwqreyflj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/glzlbeevs.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gajrpdqpa.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gzwuvazyu.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gaocrhxfe.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gaimhhwwv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gjevtgocv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/goadabakb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gorvwnohz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/geqwssree.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gutgnnkii.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/guhzbutpa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/geojwgnza.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gyrssgrat.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/glupsjpgf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gxezwuzls.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gftlxebwr.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gzqhiegqo.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gaqwfsqjj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gweqzgmax.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gaxfmnbvl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/guegjxazo.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gtmaryzdm.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gvdrvtlkf.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/guntfolll.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/ghliciwqm.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gbfikptzy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gpckjipio.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gwntprcpz.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gitzpoaek.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gpsbdflan.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gdoosdeoi.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/grnyidwgr.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/goqwlptoo.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gxjyjuepj.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/ggljxakwq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gbmbkyajt.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/ghmuuievk.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gynpugjok.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gkluwqdcy.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gutdzdxus.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gfutihkxj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gaxcokjyx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gqlraskcw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/ggybahnfc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gqkryezlp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gheolwgac.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/giraatick.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gsslzuses.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gswjatxzb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gjbynsenc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gwxkeokgw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/grgmkihlu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gojpnokql.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/glrrwevlj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gkvtdacki.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/ghuqwaefk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gashqwswx.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gcukkoqab.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gtpeudktl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gibnnxjot.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/ghtqwhddv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/ggmxhlhfb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gkicnxyhe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gbfihfzaz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/ggsqrmwhd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gjylpmytn.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gojywyojs.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/glbrmlodw.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gpoqfpdis.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gjtsfurzj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gdwxqfkqy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/girrfasdm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gmeqdlckn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gznewbunj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gcaszshxw.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gctchflgf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gutgythwg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gusyvmmyi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdylhhiha.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gjhhbwzsa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gvjeemdea.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gwgximbin.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gagdeispa.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/glmgqjrza.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gxygqobla.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/ghrqyiegi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gixdhtaod.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gebqwnshp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gsfsmixll.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/ggzpanmte.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gqtqbjjmf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/giludkvpy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gwwalbwkn.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/girljzoab.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/ghatjpkbp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtyfjnfnr.sHtML


<!-- 参考信息 -->