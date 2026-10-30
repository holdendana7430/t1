代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/giokbzxjv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gxhfqrafe.sHtML

TS:   Math.max(...arr);
来源：http://blog.fanxiaobao.xyz/Article/details/ggwtgwxpn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpscdghsp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gufihtxyl.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fanxiaobao.xyz/Article/details/gojpqhjmg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkkztjgk.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fanxiaobao.xyz/Article/details/glrtfofjw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufjfwwlr.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fanxiaobao.xyz/Article/details/gdfwucqzn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fanxiaobao.xyz/Article/details/gubgelfrj.sHtML

TS:   nested.flat();
来源：http://read.share.fanxiaobao.xyz/Article/details/goiydsqzw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyzrguok.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzsqhgem.sHtML

Ruby: nested.flatten
来源：http://m.share.fanxiaobao.xyz/Article/details/gyihduuqk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuscccxb.sHtML

[D19] 按字段分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gimtsmoyv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gmvhqexov.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fanxiaobao.xyz/Article/details/guubuhvgo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fanxiaobao.xyz/Article/details/gjctnlfwg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjlcdkgg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fanxiaobao.xyz/Article/details/gedosopyq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzdjwlhc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqgkbgvn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fanxiaobao.xyz/Article/details/gjvxwhuks.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvxhzwda.sHtML

Py:   Counter(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gdcjfpbdb.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gcvqkkuke.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gstfrudwl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtmgrmzk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpdamxye.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fanxiaobao.xyz/Article/details/gtilvxnpv.sHtML

Ruby: arr.tally
来源：http://wap.fanxiaobao.xyz/Article/details/gkrjmfcbf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fanxiaobao.xyz/Article/details/glghaljbi.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyezovmbs.sHtML

Py:   x in arr
来源：http://wap.fanxiaobao.xyz/Article/details/gwlpxzhaw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gigjaluob.sHtML

JS:   arr.includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gmrxktmjw.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkahvpfs.sHtML

Java: list.contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnkwugis.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzojilwue.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqjzjvrg.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkluhuhne.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fanxiaobao.xyz/Article/details/galagiirw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/ggbyygfsj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fanxiaobao.xyz/Article/details/gdvcujnji.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/geowajeik.sHtML

TS:   [...arr];
来源：http://wap.fanxiaobao.xyz/Article/details/gngulzlfq.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gidmgnkpk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhfpzggu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhduwvzu.sHtML

C#:   new List<int>(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqhphurx.sHtML

[D23] reduce 累积计算
来源：http://3g.fanxiaobao.xyz/Article/details/gquruvdtg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkmevjbr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwlxyrra.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/goscqozrm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabsvmeid.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fanxiaobao.xyz/Article/details/gepthcwlg.sHtML

Go:   // 手写循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypuzywge.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fanxiaobao.xyz/Article/details/glctfdxod.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimzxmoei.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fanxiaobao.xyz/Article/details/gfwvvxemw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fanxiaobao.xyz/Article/details/gtcrwctja.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gxdlzmdgm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gwuobefxg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gbgstmghx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fanxiaobao.xyz/Article/details/gzfzhowzc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gazigblxv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fanxiaobao.xyz/Article/details/gcsslymcf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fanxiaobao.xyz/Article/details/gavvwsuqp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqcbrhwu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fanxiaobao.xyz/Article/details/ghoptzndd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fanxiaobao.xyz/Article/details/gbeagrinq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fanxiaobao.xyz/Article/details/glcrygsno.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gynifxwct.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/goysjwmxo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fanxiaobao.xyz/Article/details/gwldqcsuf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvzdiqpb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gddsmmhyf.sHtML

[D26] 数组转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gopzpfalw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsloaobc.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gbsxoxvja.sHtML

JS:   arr.join(", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyqmiegx.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxeaslai.sHtML

Java: String.join(", ", list)
来源：http://baike.fanxiaobao.xyz/Article/details/gckpqlgcq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gshkydvan.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixzmsdqd.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fanxiaobao.xyz/Article/details/ggbazcgqg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzaqajqui.sHtML

E. 字符串处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmvqybuh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guixdkvfm.sHtML

[E01] 拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gbbvqwksx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fanxiaobao.xyz/Article/details/gpxpwarpc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gvoafsxgf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuberozc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gidkrihwm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxatyvhol.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fanxiaobao.xyz/Article/details/ggholwejc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fanxiaobao.xyz/Article/details/gtwrxcrel.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxflhqpot.sHtML

[E02] 重复字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ginvuhlqv.sHtML

Py:   "ab" * 3
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaayiixw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/graqdrnae.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gptaqvzyz.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeivamzv.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gasvbeuse.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpslbefvy.sHtML

Ruby: "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/gobyidboc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/geihszkbk.sHtML

[E03] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjzqyxby.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fanxiaobao.xyz/Article/details/gmpgxtcoq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwthattec.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhrabflk.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvwgrphx.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqysbnjt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fanxiaobao.xyz/Article/details/gyajbszmd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fanxiaobao.xyz/Article/details/geqfvbahi.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gegaawewj.sHtML

[E04] 查找子串位置
来源：http://www.share.fanxiaobao.xyz/Article/details/geblkdzuc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvbzthgb.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkurhuods.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gggmqiyse.sHtML

TS:   s.indexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gvccwgrpr.sHtML

Java: s.indexOf("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gzqnjunxo.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqlqqeqk.sHtML

Ruby: s.index("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gbnyegdsi.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gigqqchkh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghykdmkbe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gamptmqvl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtynzskxl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcsixnfe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamewnawg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gntqdhmhh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgylezwj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtekrhnsj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/givzumfge.sHtML

[E06] 替换子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnkuclap.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqivztps.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gdixaztoy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/giplhilad.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhxnocak.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscqhjryh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtpytpgp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gmrslskve.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gtnhdxdpv.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fanxiaobao.xyz/Article/details/gnovofdgt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fanxiaobao.xyz/Article/details/gpjgkidnw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gievnbxvw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fanxiaobao.xyz/Article/details/gplxxbetx.sHtML

TS:   s.split(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gjstamecd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gersxouvw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gcyptvavx.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fanxiaobao.xyz/Article/details/gieeixzgs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtglsvkwz.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gatxqienc.sHtML

Py:   ",".join(items)
来源：http://blog.fanxiaobao.xyz/Article/details/gwczluwni.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxkknmmr.sHtML

JS:   items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gusgbabtu.sHtML

TS:   items.join(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gwfccqnsq.sHtML

Java: String.join(",", items)
来源：http://read.share.fanxiaobao.xyz/Article/details/gozrvohvx.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gslchgpbw.sHtML

Ruby: items.join(",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjnigicn.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfhmytjv.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnelncbb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gzfplddae.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gbrbdlnbr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkikavgaj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gsdynczow.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqjyyahm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gstevwfie.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfdisicf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/guhjemvdr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcymagzl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/glergulol.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfyxrplz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghuoxxqp.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqewnydxq.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzrjhgrs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fanxiaobao.xyz/Article/details/gipiieuox.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gftimldxp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fanxiaobao.xyz/Article/details/gamiuxxxj.sHtML

[E11] 反转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gakwppsyg.sHtML

Py:   s[::-1]
来源：http://blog.fanxiaobao.xyz/Article/details/goyalcthg.sHtML

PHP:  strrev($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gllfpyfdw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/goinxjiri.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/ggtioxdos.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcrafecj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/gbgtafqiq.sHtML

Ruby: s.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzvietdj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwkrtbpy.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhhsrgkx.sHtML

Py:   s.count("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/grfcnpnhj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwuhaeyg.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkxfdlij.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giundedfc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fanxiaobao.xyz/Article/details/gokbntifv.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbuglxzg.sHtML

Ruby: s.count("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnystxptk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fanxiaobao.xyz/Article/details/gateyuvpu.sHtML

[E13] 逐字符遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/ggogqjufy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fanxiaobao.xyz/Article/details/gclaoeqas.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcmazarm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbarsria.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/grubxjsjw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gwspepwjx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpsbgyum.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fanxiaobao.xyz/Article/details/gthqvamaq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gemkeszyy.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fanxiaobao.xyz/Article/details/galxqhbis.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbopdiwm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gramvpfjw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihjzqkzl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gzuxntvgo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiguexsr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fanxiaobao.xyz/Article/details/gzstqkdno.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvypholdk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/ghulciybd.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fanxiaobao.xyz/Article/details/ghmhymnog.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gvqoiqkrs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpumuqzgv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gwflgjgjk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gkhqujewb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fanxiaobao.xyz/Article/details/gonchiioa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gbktsxhzl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gesclhzmj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvotvecag.sHtML

[E16] 数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkuntsqr.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtalrkabs.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fanxiaobao.xyz/Article/details/gemqvayyn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpptcvgwh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxppzfyie.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsayqdls.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokchnfse.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuaozycx.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fanxiaobao.xyz/Article/details/gjqnnzwtg.sHtML

[E17] 首字母大写
来源：http://www.share.fanxiaobao.xyz/Article/details/gjygyjrhp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fanxiaobao.xyz/Article/details/gprbhzqsw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gvmbrludo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gmrpqzqjj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/glbriomov.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfzvauct.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/goyesmfya.sHtML

Ruby: s.capitalize
来源：http://baike.fanxiaobao.xyz/Article/details/gxobckeuc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fanxiaobao.xyz/Article/details/gfkbgggcg.sHtML

[E18] 模板占位符替换
来源：http://blog.fanxiaobao.xyz/Article/details/gylrajxnx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fanxiaobao.xyz/Article/details/gbatmsekf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gimqmneuw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/geuuqeedg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gukklmpok.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpntixsks.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwvezvlu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntmpxdqt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gupeqhosh.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fanxiaobao.xyz/Article/details/gdcnceqci.sHtML

Py:   s.splitlines()
来源：http://blog.fanxiaobao.xyz/Article/details/gpsymnmrg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gglrjckhx.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryswjxrk.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghchapfsk.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzljvrii.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaiiqgfj.sHtML

Ruby: s.lines
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsfozwmi.sHtML

C#:   s.Split('\n')
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkokobuw.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fanxiaobao.xyz/Article/details/gazziumml.sHtML

Py:   if not s:
来源：http://wap.fanxiaobao.xyz/Article/details/ggjwynngl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvwhgher.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzvthixnm.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guykowabb.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcdszilz.sHtML

Go:   if s == "" {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpntpznho.sHtML

Ruby: if s.empty?
来源：http://read.share.fanxiaobao.xyz/Article/details/gttmwezss.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbryhykfm.sHtML

[E21] 超长截断加省略号
来源：http://wap.fanxiaobao.xyz/Article/details/gzjfgsmiq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fanxiaobao.xyz/Article/details/gvttquseb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/gqqwaqywh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gqanccehs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gfolfvxpo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gwhzetffo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fanxiaobao.xyz/Article/details/gybawxevs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfnrheme.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcjghoch.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fanxiaobao.xyz/Article/details/gumpbwjxq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjanfrxga.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibzkykyl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzfqoswc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gpqgohhxh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/ggscsxjuy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grznhcpwd.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gkkfqcxky.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gnafmwbxl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmxqsarm.sHtML

F. 文件与目录
来源：http://blog.fanxiaobao.xyz/Article/details/gxyjmqisl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdghvvzvs.sHtML

[F01] 读取整个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnuzbysq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfvcuwcq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkwmrsjb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fanxiaobao.xyz/Article/details/gjkznkobj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gsxuieaps.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gkyoyvvwb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fanxiaobao.xyz/Article/details/gdcitbuwx.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcglbstym.sHtML


<!-- 参考信息 -->