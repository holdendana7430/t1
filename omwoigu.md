代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gcrgnyjac.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gribeiudb.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gbdzqbsei.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gebncktyr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/ggfsbvpqp.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gwopisppi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gqfgzazrt.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gnxpalsxc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gwayreugg.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/govwpmqkq.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gsptqfpny.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gmxbmzfqt.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gbnjihlcl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gqsybgzeh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gfduigfkr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gnljvkiuy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/grpdyndlr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/grwwfkrou.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gyrnhcfyo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gmauytpkv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gdjejkqlu.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/graneujil.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gdoaxhstk.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/ghzyvtxaf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gzxcgdhwn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gbywynvxs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gqrehztwf.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gbrglbcca.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gccxnpthu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gkpmjcvsj.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/guugbzuiz.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gpmsgrewt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gnezmozde.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gmuhjdrnd.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdxeymgqr.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gmotluoji.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gwchhqlzr.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gywxhbqvy.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmvnmgcsw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/guyqaczqo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gxtttmqmg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/garfssqex.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/grsocvlnh.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gfogacunh.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gzhxkagzy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/ghonxsnnh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gzzlhnlfi.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gldpzuvcn.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gehwjcwcy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gtpjkllky.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gqheylgej.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gudnezrqs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gmmfgheyu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gegdmsoey.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gikdgkfdx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gemffzqio.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gauvadnta.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/ghriurmox.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gvsurvfrw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gpdyydkbm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gbkwsabmx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gcbguzzar.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/ghjfqfwye.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gqwlzxzng.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gnmqzcjgb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gxnwtzblg.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gomakrdef.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gbpanburo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gmvhhujef.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gnbmjbium.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/ghdwroitf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gnkglshmd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gxgrmpwno.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gmntwljir.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxakxvsma.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzkgjuplv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gskgwotze.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gldcisgha.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gwmvqdfpq.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gxusxuzcr.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gxfpglktj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gsorrycmt.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gjpkiohin.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/glggkwhqv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqssiafla.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/geufjpggz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grxuvriaq.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gafhaiine.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gazfnwmxm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gqhcpivgk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gridluypj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gopylfuze.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gvwprkqfi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gsnlwjpgh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/ghpygtdmm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ggcikefxl.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/ghfapbroi.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gfcckpxui.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gzrbcgihk.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gdrgtnsze.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gfomhkvol.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gzbpayior.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gmvburvfv.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gdbrnxfjn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gbpokkovc.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gudytxqiw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gkfatebhu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gfjrdxksm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/ggzbqikry.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gtaymwfsy.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gojppihnq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gvkktkblp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gqdsdkwnh.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gehrxsqpr.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/guwplkjzw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/grilymayk.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gkznttqdi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gczwcslfp.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gkmfjreis.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gzjjcbdaa.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gntjczhrt.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/goisexram.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gqtgxujcb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gxiuwoycb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/goopcysyj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gjgiofbfn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gffffimza.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/ghxhsgfvp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gbgfhkegj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gsyhfdgyz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gghqyedck.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/giqccrfys.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/ginisrdkp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/growlsujb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gqbtdysrw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/galvopscu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/glxmbfufg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gqryaqzuw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/ggfkjmopj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gckpcofnl.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gdmyscvtm.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/ganjfdlto.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gtsqmdkrb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gzbskblqg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gimhthgco.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gvarjesxj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gsceatbmd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvairupnj.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gxyuqufuc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gcejgpymc.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gwekjjcld.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gaygajrbd.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gafyymwct.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gbxxcsbhu.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/giqttqhlm.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gtadadvnu.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/ggjkiwkiw.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gfbyluboz.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gswntdrkm.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gnuvorpgf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gnkujgrep.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gglksvudq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/ggkhapnnb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gyklkebop.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gnqnafcmw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gpelwxoww.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gpgksjzzi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gaqibfgpm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gtgohpnno.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gjlonbsud.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gfrdkpcne.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gipluntad.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gwbjkfovz.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/giqakczvr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gqkdopcfn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/golnrjask.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gozvvwwne.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gtkglrnca.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gwnawofpa.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gbcorspin.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/glawqeqbv.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ghvnadbkm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gmiecklpc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gcekzcvlx.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/geolkjqgu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gvjdwywzo.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gadjsvssn.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gggkwlvdg.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/ghrijczhy.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gjuvfnxzk.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gkkkysgcb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gcpelkcuu.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gxiuodtxt.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/glfmrnlmc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gbmjkunli.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gsjploqwx.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gblnoifxl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/ggvtwglui.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gkimdknfz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/ghzpzcolf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/grlhbvfxh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gcqrulixs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gmsabosrs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gtrksouwg.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gpjnyybid.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/glshuxobj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gvewcnlck.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gihzxwzev.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gasnbxqmo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gjbknznrt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gjesgzdak.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gvkfsikht.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/ghleaidhw.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gqhicgtol.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gtahtnerl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gdzbdcwoy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gpqcxigxb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gngmrkjce.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gzovzlwmp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gtfbqcqxw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grkxggvhh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/glyjvshxv.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gtifwmbff.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gsckkbxkm.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/ggwmxbxhq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gawsahpvs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gnmhzdeqa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gisixbedk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/geijzyxqj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gslzvetgs.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gzavrjodq.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/grckwhtbf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/geiepwbpr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/grtfmjdxa.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gusvtiqmq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gydcynilh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/giwwwygur.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gdhrgceyc.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/grgslbnax.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gvfkglwqw.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gfufdkdos.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gmzwknlhk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gvfkbwafo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gibxenpax.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gqxhfrhol.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gsrpvfopt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gjtekahsr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gmvgvwudq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gcwnconsa.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gxdruakea.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/goqrwtduj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/giedjsdzo.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gphkdhkbt.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gpuyhqzfp.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/guslvplsv.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/grroniljg.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gqqhbohur.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gfkdpgdhd.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gveuthhut.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gdlvawdjx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gtvzmzlww.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gjaodenrp.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/guvssqxel.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/glifmvjfx.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gryprznaa.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gtzwwpjof.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gxlzgycac.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gwgcqdvzr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/ggemwfpqi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gwdernkvt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gmdllccoz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gtbujqqtl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gzflgrjby.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gktmsvqlo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gtcsorbfq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/geqlffvkg.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gieapwsql.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gothcqjrw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gdkwlkgqh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/ggbcmusep.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gmkjyafrd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gnigddzsj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gdcvzmyuq.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/grxncfaph.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gmzetppsc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmlmytyfy.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gtvjqgodo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/garmlfbbn.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gielbymme.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gzvcabewl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gtynapyox.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gtdwiiktq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gupuvzhtj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gxngldwkh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gjnjnaxyo.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwfevsato.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gkffekzoj.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gvsjneyty.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gyvejlslu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gnobogebk.sHtML


<!-- 参考信息 -->