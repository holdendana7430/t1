代发 wailian999

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gjgwkhutr.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/ggslajllw.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gsfbqyrfd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gqyangiqd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gutjhjclx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gziichcig.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/glqqqvdlt.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gpevgboeq.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/ggeisgkuz.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gsbeuawrx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gryhdnlrx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gthyytaya.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gnuqsdvcl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gatqrdttp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gictwrnlz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/ghcyjbsdc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gnzmuyyde.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gqriicnpp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gxdphawsf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/glwlyfcri.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/grkwwzemb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwwobtvhg.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/grwnyhvyq.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gsnchzpsc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/geiafoocc.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/ggqzijayd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gxtrtzlct.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gvvptestz.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gpttgfabk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gprbxsake.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/guptfffri.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/giftngetx.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gxxvwgibr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gpsozrcsd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gtychqymv.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gemjmzeas.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gqcmsrvjv.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gjaducxrb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gvytgjqgr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gfiasxibe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gwyrvapix.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gzoxxjguy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gbeyqhapw.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gmbicuxqr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gqhujagvd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gmrftqxlu.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gfpnlgrzs.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gchavrkur.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gaypldvzu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gquykfpvt.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gausvweud.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gxdvvzkwq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gowqfktny.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gnuytqyqi.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gepiryqmu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/glpgmvepg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/grgwpsiut.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/grzbsydwn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/giuequgeg.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gzsiqfvfn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gtmbpidfa.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gtfcqtfua.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gmsqtquya.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gcyqlnics.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gpqdamuot.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gzvqwrdzo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/giacvuroh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gcjbajsri.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gimbhzaea.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gkbjxhspv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gikwxlpiv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/ghluexsqo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gmzxdoacu.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/grsiulwmc.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/glqtunftn.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/ghvsakyfy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gxysfbtuo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/guwopnhuv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gmjknfndk.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gtpgkybew.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gplyjwrsr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gwhwzoolw.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gyszypupx.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gtjkxpfkx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gxfyextdn.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/greyzuvfm.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gbmthxwan.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gzzvzslqr.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gvuclxutu.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gnctoudsj.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gbdihhzql.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gtjuxsjwi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gsmjwotmq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gkdaocbuh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gaphbbasn.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/grvroryav.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/ghjtshzsd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gieqmgyuz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gvkbdaifz.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gesgawkyx.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gwyajcwtx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gedbttbfr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gfnfhabcz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gljcexkqf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gyjphbudz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/ggbtyqezo.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/glmpngwrb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gxjkdmbjh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gocgnxdcq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gibqsrpjw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gpdtgetsj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gcaretysv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gsauovomy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gcpjiksma.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gwevkxlin.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gumpdemnu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gddcaping.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/ghyizuoas.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gviyvmrhl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gukowfxpu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gkjngccsq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gpqtiqhbc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gqmxravpr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gmzknunxk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gbejjmzrm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gqhrudhoo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gtyidkbej.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gxitaqbwy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gyknzesep.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gcgtpypqi.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gvjahbliu.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gleoyxfng.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gjisywbzi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/glqdkmlfg.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gmbfraqbo.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/glknzmgxr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnmduinfc.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gbnyxbkkn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glpntwdas.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gglpmgacu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gviubiigp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gruxyhpgr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gdtoisshj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/grfcorzgq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gkopmpwyg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gnuccqcra.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/ghqwiiknw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gtmvybxte.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gweguvdqk.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gbjuborbk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/glphxqwga.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/garskyurt.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gxuikyxza.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gkalbodmi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwulsoyga.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gebchydmo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gdsudcqrw.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gdittcfbh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gmdjlevtg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gcygmdsmi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gjkqegutl.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gmeljxjyo.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gzohknkng.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/glgfwgyyi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gidewwtqa.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gkderozug.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gkrtecxjr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gtufnrqgf.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gxrgzzrwd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gyhffqnxi.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gltbruyww.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gaotzmnun.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gjnmmddel.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gusntynyw.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gvaivjcrk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gvslfdnvs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gobglxnip.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gxrydzbin.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gfunbodcv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/ggvbsngqa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gqalczvgr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/grityqamb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/glsqqqrtj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gqzbdqxct.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gbnrnfwiq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gwvffknhf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gfcjzxltg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gzvzqprdh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/ghiiznucg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gywuijcvk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gctzmxrxt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gushapzep.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/guiatnpfr.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gjggltvvh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gtkbzqysl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gumtvdhdl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/grnwhrxgt.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gukmfrucx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gxdwkldnq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gbikjvtwy.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/ghbshhvdt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gzvtwkmgm.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gpfxubgwi.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gwzpwtqba.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gqnumipor.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gmlhjzmja.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/geifuwfyr.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gevhtiaoj.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gxfmizlbb.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gejxpgoat.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/giqkflyei.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gwgceaege.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gjtlmiijv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gvksrgjvt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gicghgkso.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gamueoeup.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gldqqpdxp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gxdkqslgl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/goumzkhwx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gvdiivkcj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gfyiyoyfw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gjpwideoz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gujqmemai.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/giidgmhbo.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gwqwyffkp.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gfydkiafi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gkyxbaxvr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gknfoaium.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gvtutbpzm.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gcfpqhruu.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gbxhbwbfa.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gpmzjzwhm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gymlkbbzf.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gmyhqecql.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gfiqvexso.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gdosbnemq.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/geobjcqda.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gmbxqvwwq.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gogtayfcr.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gthdruguu.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gclibynpc.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gxeipoyjn.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gtmgecsqz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gqsgalcsb.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gahvahoak.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gpnrxfrbj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gwkxifnrh.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gbednqjab.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gfoqrakta.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gddelrziw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gcqwnkvml.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gozojldyi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gamlhqwem.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gxxdkxqjb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gkpzkvszd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gqipjpont.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gprtcforl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gokjcjgom.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/griidnusc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gjtgpwcvj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/ghifihuag.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gcqrzhckf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/ggutegzar.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gfsckaggq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/ghxmwtxkt.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gxqrnlmcb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gtxphlmxy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gqilldftb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gyljbfizm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gvgcanagp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gvepmhybl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gwfxsfjlt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gsycwbddn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/giqxvajdf.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gnxzjyino.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gsiogmiqd.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gmwprwwht.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gqvmkzjij.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/ggvjwjhtl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gbxrqewou.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gbmpjdapn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gbhbzmutm.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gttbyhzda.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gskejulgx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gmuyhutcr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gkmroufsp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gjouhyijj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gmjqtnczc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gzkezcpia.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gyplqwvwx.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/glnvvarmc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gfwccojhx.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gmnfoyohf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gvrsmuxgx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/govqlpmkj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gyxkujkaa.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gofocfzpb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gxufixrab.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gfzopfamo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gyurkewwr.sHtML


<!-- 参考信息 -->