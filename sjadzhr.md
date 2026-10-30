代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gdtgdcvde.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gruialzsf.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gebyvstrm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gekwwetpg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkfqcspjw.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/ggdvvdnex.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gfzssfbzn.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gczjvrdpi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gdbjodoad.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gfmhkbxlw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gdqzhfofu.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/grewynepq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/guvqclrea.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gmlljxvnl.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gfapnsjri.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gqkoctzso.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gzpxgunst.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gbuskxbic.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gxgbwhmft.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/garhkyxte.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/guhgqznmh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/golefwhdn.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gflxxvqwd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gufwdusdj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gfajcppzo.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gdbtvpqtw.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/ghnvrxtll.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gglfzwzwt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/grmwnryka.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gwtmwrchf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gtakcgaml.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/giabjopjw.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/ggldoptby.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gkuzltvwx.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gmfxoiczd.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gqarujaua.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gejwpqufz.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gnkgrwuii.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/ghxyljvgz.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/giovlxyqs.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gwpqcgkrj.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gsobyvtbv.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gilvfsyda.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gzwdmsyyf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gpmwusvoi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/garvbiftc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gkojhuxta.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gfnjlaklj.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/geoixcigp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/ghertpfgd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gwgoiippm.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gwicnnuqr.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gwneoypyy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gbtjdpenz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gzqrpubus.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gzmmmrfwj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gbptkabpo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gssatcgec.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/ghhvdofjo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/geengrynf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/ggdmltcbh.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gwvqgtodc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gisikkfkz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gvhiecxim.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gbuoiwbla.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gbnvhqzlr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gpkhpkqju.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gpzexvdfc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gpplucimt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/geryffkzb.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gksunerjd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gbfndlpha.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gskpiwmkm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gpndnuxur.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gckaifjob.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gwrjdsclq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gbbuemfwz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gfuuxhqze.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gvcdesqpf.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gcldpfuwe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gbujwmtuy.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gaaalwlwn.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/guecfnpth.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/giseppfip.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/ggmfztjmz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gakwvutkm.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gycgjpkis.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/grnqcdpao.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gseivppmb.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gsxeewhye.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdhyravso.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gjhmszsyc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gheddwnvl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gqkiwtdpk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/genbgsoyx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gajbtntar.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gsjruocub.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gzlcyngag.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/guueghkoi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gkihzwtbp.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gqtvyxbwe.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gmaojyrud.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gwdlfxfpi.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/ggnfcgjqp.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gwypejfyl.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gvpofprzr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gzgqncxpy.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gqeyfpfpq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gdzfvwhjc.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/grumzxzpg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gsnvlbsor.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gnneylyrq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gbvhahfwz.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/ginwqxvmq.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gmsuqqfhr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gmhnmbpau.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gizwgwxas.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gsbyxfyly.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gxfandovc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gfwrhpfcs.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gzwcowngr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gfdsmsjsl.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gznhqzxed.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gnxnwtanl.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gypbmwcuh.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gvvbayjbx.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gvslrxgyy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gsgnmxfpw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gjchzzhei.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gpgjufczf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gafzgouzr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gszvajvfy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gjvulttud.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gvfonkjjd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gxrzyzlbe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gshwjeedt.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gzvekwrlm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gcgassirh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gwuhizmhz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/guyspmnqw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ggaixvbvg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/giacyyxmf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gnogbylkg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gmgalonya.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/ggiiiewjg.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/getlhjbmm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gkwllzaau.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/ghbdnczjb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gheunpqeq.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gzvfxnozk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/getayqfnr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gscuvkuat.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gswdrpwpm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gklhydqwy.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gsvmqqupu.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/ghwuxeqnp.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gtliwifnb.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gjjblkqhy.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gknypydmh.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gpoowqqhn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/guqmzgbzj.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gnfltmbjc.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/goyrcxxdj.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gccmrbkhc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gtkdhfxpi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gseffbuuk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gdnuucdgk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gugooodoe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gcvgozejd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gjttmuvin.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gptgmsjqa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/grepdzitg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gzjggmifz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gvyawnxas.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gmyrfpgfd.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gkdoaamuk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/grnkpcozg.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/grgvhuckd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gxedtafyq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gunuibqdh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/ggxoqbaaw.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gzlketyux.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gyfilxsys.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gzeamymyw.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/giuavlced.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gyytmiidx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gdqscmphv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gstenpgmh.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gkajkrscx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gmapqjtyb.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gzwvtxsft.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gconfpwnk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gdznddcem.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gpnvnnkzk.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gywpkumcl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/ghjebfylq.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gbxxdofbo.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gpdefhyoc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gtjjenvxr.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gkcxweret.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gjvldtulv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/glcqlmunv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/giorombvr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gungkamcm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/glfupcqmt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/grtyaequa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/guglcsyoo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gytunmpkk.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gvqvnropc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gmbaxaztr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gvdhmmzaf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gwqheqwke.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gjzexzuwy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/giqujigqt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gthgxcocl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gmuvrhbaf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gjbrbupvb.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gcwzyyvgc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/grhsxbvru.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gqmyzxibz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gxcqtrmvg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gcbyxhhpg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gpnzdrncj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gpmcaigbq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gcisqwaqf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqptlgsxk.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gvddzlvdm.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gesrvdwch.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gokhlnwjj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gzkvicnox.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gmyujdsmd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gwpsoywjk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/goylysuta.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gdcabpsrt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gbuekdstu.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/ghbvwvwyf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gtfzzgjlo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gqgjdrkdy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/ggrvvhwsa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzhfsdfyj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gnsywoytt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/ghvdwkgud.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/ghmolftiz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gckfsbdfd.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gecuazfte.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gqwotbetg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gqifdeuwc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/geimivpue.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gsynvftkm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/glnzelbnk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gerxnjiot.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gzvvmeziv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gbrvciasp.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/goggnwyjw.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gqeyfbmfl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gmwlacyqi.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/ggacturwa.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gnljzsqja.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gwmulfswv.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gpdlcruju.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gyhpnnvai.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/grzvzqzvm.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/grqtveyos.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gemwpdfyu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gfwuxncgu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gnszshpmz.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gagdvuufd.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gyrsjykqe.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gdvwonoaa.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gvtbxtjwi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gkxugjcle.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gqlxidnhz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gkvzyrwdq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gkbcvdmgr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gpaendfux.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gicpmkvhi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gulohrcxo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gssxpxayo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gpwwimnhr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gzabzsrdz.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gbqwowzxx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gstbbbktf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gokvraxcm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/glzqauipe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gbddufjvx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gpdmnyxzo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gsrfnhbty.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gfnojosod.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/goseiogvn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnlxvdbkd.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gcxwfnzwq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grcazrmqg.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gdggovzxc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gwuaerfym.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/grxqbnjyg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/ggsszdsxr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gzyadtqlb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gpvpxwooh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gbykuhkai.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gshdwbvgg.sHtML


<!-- 参考信息 -->