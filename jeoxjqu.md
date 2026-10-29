代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gdnimzkgj.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gkzktwjuj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/ggzszqckp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/grjqqgyfb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/ghtxwxjbu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ghaxkskmi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gelotbzzy.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gbyatyook.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gntsagrpg.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/grnzbslwx.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gjnvqbmvm.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gpnhkbgbr.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gjnmnytlo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gctpsddid.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gvsrbrwxe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gcjnpmsec.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gqvzfkjvg.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/glqfarxbw.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/grslnqfsb.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gphaubppv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gavlfdggl.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gmlksfwwr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/glojdlunj.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/geribcqir.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/goskqyrzh.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gljrxbaqb.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gklmqxweb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/ginarskzw.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gjnaajrhq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gducchrdo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gteumpnxx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gxquqykvf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gkevmawfz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gppyapiqp.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gudkqjlyt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gjbnbudph.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gwrbcmfrg.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/ghhdrgjkr.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gmkbhbwfn.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gtvlsguay.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gkysghley.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/ghmzkmxzo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gnigejwki.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gcfcbeyog.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gcyqpdrvc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gnignahkc.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gmpettnxx.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gpxnoblwe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gewcmaimk.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gfqewdwyj.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gstzlahft.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gtzjmucqp.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gfgdzwtfh.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gigqdpwql.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gtedycivp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gciamkpms.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gvbmlqndh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/ghznprddn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gftvdjkea.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gdwclzhrc.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gcgjerngu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gjderfhcn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gticycanl.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gbqiyseqb.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gljvxwtty.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gwvsxlorb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gqapcuhdx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/grgyvlhfg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/glzvhhkhn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gyfyhwmar.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gtgcuanjf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gxqrrrdbl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbxhqzvyj.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gvuhyaepe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gkoefzrdt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gxqyryqho.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/glehumnke.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxnuiervs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gvdkayaxy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gefzwtqnz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/grlulloiz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gwmcbiqfo.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gttiacdly.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gcqztwwio.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gbhyevgcr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/glvacbhci.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/grzgtakpj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/geratmyam.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gvuehkbsc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzcbvars.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkshnkqap.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gclhtacgj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gqvjdkvjp.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gsrmctaxr.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gtkoilxlt.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gpeyyfjit.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/guofvcmkx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gsxnvygqf.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gxyvfnrvx.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gzpezrksh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfovujlcl.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gurdiplpa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfxbpsajy.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gtkbkcplc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/geybuksfu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gdtitlveu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gkuddwvka.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gywsmtuzp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/giecoubod.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gryhwhjnq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gpcpnlwoh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gppgcyfai.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/ghtebhqok.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gapiczfaw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gxjijvygn.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/ghzrzscme.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/getpnkeby.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/guwsstvbv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gxpvmtezq.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gmnbbgpxr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gzubyvehi.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gkzfbfunv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gaihiuctd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gyidwlpnh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/grajnuxbl.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gpiplykwt.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gkfgahuhu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gvnilkrhr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gnemdbadx.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/guxqykfsc.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gowoasuqs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gamtahpgf.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gsdhqebxo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/ggzemffjj.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gbtnvstug.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gwwtsxfbv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gvthkukga.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gaweaufby.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/ghcmoanab.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/goetmmifw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/guvccnyyi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gmxaxsfzs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gqlnxeukv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gmkdqfnjn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/govwjqpwm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gfkvsgzbr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gpovkskgp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/ghsvswshg.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gwntlegpe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/glunvgloh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/ghbonnrsw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gkedtiudn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gjeaoemrg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gmdgwcxea.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gyqixpigi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ghpqxtsmy.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gnjcxynak.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gbsmvhupn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gdtucgkbp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gkodrfobl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/ghxswecuk.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gsxnlxsac.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gbaalwofx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gekwpwwei.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gzhmmaqtq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gxvkkupzr.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gkkmhojyx.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gcunxqtsx.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/ghfoghwkb.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/galedjhwg.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gbvjsdhrc.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gzhzrrhrz.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gvvyvcoxp.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gjsmexcou.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gwlvhytwr.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gdwuhjkzf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gutqgujbi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gzysskhrr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gokzoqteb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gabqadyll.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gffyfygur.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gjdioaliz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gebvsurff.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/guuhzyjzk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gosshreky.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gijrspptg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/ghcwiilos.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gieyaexwd.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/goptqevwc.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/glernkofs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gsmgybrml.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/grxlgenpu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gcptcfods.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gmhwzyayv.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gosysciub.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/ghlrhutlh.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gkygcvepf.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gkfdghifv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gcrtnspbs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gncwcxyoy.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/ghpvigtbm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gnleervbt.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/guzpkbcvf.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gohlztbkv.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gkfvgrkem.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/grwxrrsmt.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gjaenqdtz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gfesjxyuo.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/garpfhurf.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gfqrgaldj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gvwioawhz.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gcyhyopha.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gtvtqnmub.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gxtrrarfb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/guhjfweyr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/ghvcinbtu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gtdiuppbq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/geaopyypv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/glyabbjaw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gyujyjzzv.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gslkisbiu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/goguggwwc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gahkhcinj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/grqprhrni.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gulztvzoa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdanaaaw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gejehjott.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gsfnabjri.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gvdyqcxmt.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gpaocvusr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gzeuqbllu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gkbkuujes.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gnzagdkix.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/giukuisye.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gvliulcax.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gluuesgze.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gysiwqnwb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdmrfoalw.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gqcixjagy.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/ggetfllru.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gqawzyakw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gerwtavpy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gdeygnkjr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gutsboais.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/giptsyder.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gdoexzbag.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gnpfbgffc.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gwsqvqmgl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gwpxlhlpd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gqvxjhunq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gzndamnbb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gjlcazqtv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/guodqznbi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gdvwbekjy.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gwrdwpoft.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/golmmnzwv.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gkkgklvut.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/glqqeifei.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gaxepigsu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/giqwatxch.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/grvgdzopg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gzakavtyd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gahncijdb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/grtumqidb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/guqssezmz.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gplkkifvr.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gslscepuz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/ggjppemle.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gvmqdwfxi.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/ghcmzcgss.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/ghqbzcmzf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/ggfssersv.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gwmrqyzix.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gbbhnfrvy.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/ggfxrppck.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/glamcwdvw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gojuvxmtb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gxuslgkvb.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gizboabzw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzgyfvhmh.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gikhrqqdz.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/grntnkwri.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gbcuwxocu.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gwhlvgxwe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gawkbrdoq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gixoroxoc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/giylkgqkx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/grjrbgjkb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/geigvrobd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gblwfnvip.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gwxjijifp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gpjvnotmm.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gxmvdhfsg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gekrpaijd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gjdhgwquo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/geponvyyy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gesxpusai.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gtbdwamld.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gtapqnymj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gpgkvwwex.sHtML


<!-- 参考信息 -->