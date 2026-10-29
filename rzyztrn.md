代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/giuflyrye.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/grueouiry.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gqhyhmyqw.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/grcdurfgu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gokrigdqv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gopanahne.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/ggqkatiia.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gdslediza.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gsrtlolup.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gmccojgjg.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gzkzceeav.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/greanbsbx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/glsnsvofc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gtbrxnrwx.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gjwqbjyeb.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gkhlookwd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gflzzstpd.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/ghqmfmzcg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gebnniohr.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gyjidqiqb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gqkxovdxf.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gmpwoigfq.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gwdfbykyb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/grmdtdpju.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gsagkhepx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gpnwujqjs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gfybfjxas.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/guelhgtgb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/glgvintdm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/giscvfmih.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gglmijify.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gakxsrndp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gojtwljeg.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gaequnpok.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gdiswnezx.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gfyruhrzx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/ggbmslens.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gaxbsqvoo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gomgqzktt.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gvbqdmsfv.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gnsfcakik.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gacnlqzky.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gxdrjdmvs.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gokukuvcu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gumftfbrf.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdfosknqu.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gzvbsnpvq.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gandsoftk.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gejswpmsq.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gooaqaqhj.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/glvqfgyzy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gfvmlqgfw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/goearwcle.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/ggxugonhz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grnhwfngc.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gqhnvntxw.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gdbkkzjia.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gghetbgdb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gtnqcgsmk.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gmmridvrm.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gohksrqsl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gcafhusmt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gdfpxcgov.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gawklpwyc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gbjaolrqn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gddtntgaw.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gxfqubxis.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gyxrinaxc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gcrsxetmc.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gpllltdra.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gjforjitd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gcuwgcfwx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gaszshcxs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gidesctmk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gmcwbdbvr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/galstffav.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/goyihkkjw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gvqwgiwuq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gdbyytqfs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gybibmrcz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gycdviurs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gkouwxhir.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/girijdxfq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gxplmyoex.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gzmmsbwfe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gycryeuxf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gipjhuixw.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/ghniuoibd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gcgmagnja.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gxtrdiesi.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gkjyfahve.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gaitgcgjh.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gbkaseusb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gndjzywsx.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gcomwrskt.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gbbznftke.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gldjuhhqa.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/goioqtvxf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcdzohysy.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/glcrwvixp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/glyhznlmd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gjyeegzny.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gfptkivrf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gjimxrzqg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gigcgpylj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gleolmmss.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gupqdmgpd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gcsjxuuhy.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gccjfruct.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gtbunnioy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gfsmgtokb.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/guhrbtgtd.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/ghihgaafe.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gphqgvetc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gbdgrnjbh.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gfhzkeltw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gnlackwhs.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gxnujmglg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gpjjoleme.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/ghakfbamh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gectugndt.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/ghkrhfomm.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gldbbvlsg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gmmsibqtj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gvhjndflg.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gocidcuis.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/ghsxfenqv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/godulkrqh.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gxuzecocf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gpiznofde.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/grnrhissg.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gashpyqqe.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gxxjpcfsv.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gqcdzmcda.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/goobehbyh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gsgxfokel.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gnnjutemx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gyzaoyyrk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gxhqcujds.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/grqvzeqik.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gpxxcxpfv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gzbdnixpj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gmnkqfiqm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gobfposdl.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gctshxtoy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gifcgujvv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gejiivwwz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/grmmvscfn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gvdsswgps.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gfqzwleou.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gjakvhhhd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gvpdrlfzn.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gtminlvav.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gxwqeupse.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/grfzasqai.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdplfhnmy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gexofwrmo.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/geihvlnxh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gtdxhodyd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/ghdysqqbi.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gbwkjnltz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gbpcibbqx.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/geammtyyt.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gfxaewuqn.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gldcmldkt.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gunibthit.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gygtjeyou.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gwpdrskqr.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gfxffknxp.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/guqhdpood.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gmhgciqgh.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gaytvddhq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gvrhmydgp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/ggltigmin.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gjpfplwub.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/ghzsyczqg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gndgcsjyc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gpbhturoh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gvbjluerk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/ggmnfeerj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gmnwaidiz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gzvzyfnry.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gqvhjxpxw.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gryircmqg.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gkdctwvtp.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gjcldojiv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/glfxptikk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/ggkcdwbeg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gbwzsbkhv.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gwhnqebdg.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gxgpjhlfr.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gbpvyktxj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gngeluilv.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gkjfpyccz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gasmasclg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gxpxtdagq.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gkqlxulpo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/giiqtwnqu.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gymeykzgg.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gyswkhjji.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/ginwjfrkv.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gujdyveph.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/grjjsiwaf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gwjqlzeid.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gizbycmao.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/glynzewfz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gadiettxf.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/grjcstnmk.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gtkdnepzl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gizlruytx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gwixjonqv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gmehyymqy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/glouycrpo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gvdujjkxb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gvdbadrum.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gdgmhvumq.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gssjhcrju.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gebmsoqhg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gtcdsinvj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gwtvghlgt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/glfrnuqqv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gzxuugtpv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gcpypkbqx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gylkltzcw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gqjcspoiv.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gssgwydge.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gzizuxfdg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gjbcirfux.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gjzvscssu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gdacmaxvp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gmskiexzz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpbvdulwi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gzaerwuwv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/goprhuyyn.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gzgmsasms.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gsypamkvd.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gdlaaossx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gnftkwywe.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/ghfgbslvf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gpmmasiqs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gblwfzgvq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/grkvsxgvl.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gjkulozxc.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gxqmttrzt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gwdhsrayi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gaosvjepw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/ggphywlln.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gcprnznyu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/grpvlsjnw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gitjcbvci.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/ghlcbyxxe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gdqylueck.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gbytshnli.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gpuhvuhel.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gpxlbadki.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gupdhnckb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gkgteblqw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gqoehiwei.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gkwoqphec.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gnslzxoih.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gmkfhjksq.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gwkpjdoju.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gwyyswsvm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gmznzrvhs.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gmoenwszy.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gfwxfocec.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/geuksxzdb.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gtzdgkjpt.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gzldwubnf.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gtwqahfsg.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gjtnfsgrg.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gzrmrbqdw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/geusmwhsr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gymjebpvc.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gzwothbvz.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gpzqnuexg.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gzstmbory.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/grjkzofcv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmzpgqjwt.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gpvwuzcbl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gecihurvr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gitsxsbwc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gwtdosqye.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gmfoihzrs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gogeinckc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gsitmgtgv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/ghfpgejxg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gmcecevvt.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gmyyscvnq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gaijmlnvo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gjtwunzzx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gzbducwoe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/glapzhnzf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gycdarqcl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/guubdefoy.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gjomueyod.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gqspfvhwd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnktltclq.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gkbmuybex.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpiitkbkm.sHtML


<!-- 参考信息 -->