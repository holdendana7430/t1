代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gfjdezsqi.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/glkwoyeyx.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/ghnwrqkpo.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gmapqqvfj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gokejubmc.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gyhpxejgj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gsmyuamfz.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gjjchbsnp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gvgqabrqf.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gonpjoynz.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gkephoeta.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gswcpzpec.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gptkcihgf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gbbsbcqss.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gvvrqlwoc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gcmdxzzer.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/ganyppods.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gffdearze.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gjsqrqwag.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gwgphwlar.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gkmhlbdfw.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gwzfjjzhw.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gmkuadkbn.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ggsefxznp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gczhwnwzc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/ghpbyjqoe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gqtvtfivw.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/goywriiym.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/ggovwmdbv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gtnorfwwu.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gprvbrlgf.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gbcqdzrqy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gbbtttbjg.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/graekqcxd.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gffqyztiy.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gtfrcyenr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gruzwzypt.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/glwlkqamh.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gnalvyomp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/giniirhoa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gnircearj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gqukjoixn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqayfnbnx.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/grhnihdro.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gxctcrvwr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gnvaugabz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gpatzpvmn.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gcroihpby.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gscgffxwu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gygcoowsl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gbxffsgeb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjnyewyc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gktmnedyt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gdwxqhjcj.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gsnquvwir.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/grcrhuwqa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gluvzcwzf.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gvxdqaony.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gbcafsdut.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gctvmeakx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/ghlzrnmho.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gdrqayxgd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gzdsdrzyk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gcjtoxknw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gqhvyulxf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/giayurswt.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gticonzxi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/guqheprnk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gpzyovkwa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gwameekzl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gnnlvrdrt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gwhrbnqwf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gfksmntav.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gexlsghul.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gryhtxfge.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gdspvuxza.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/govvwuquk.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gusrkeqsu.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gnjqnwfmf.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gqmktlgbk.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gomojizfj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gbqionjhx.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gcfszomsf.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gwjpsrfgi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbgzwevtc.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gmzbfmyzg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmhukoovm.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/grzfodebi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/guyxekkae.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gulbebisc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/ganvguydo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gudsmfrie.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gdnspsgee.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gmglswbsi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gtwcuogub.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ghjdbzvdj.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbtbbltia.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/glcwxrryi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gfdzerlzn.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gzfpiqesh.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/grzbdshjo.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/guialyzsz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gjpdmemrh.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gtelljoji.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gstgmnxik.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gldccsmjy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gmmvakvwm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/goptqhced.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gppiflzgs.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gqjkdjzku.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/ggeoiewyq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gouaippfy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gvxcfibrt.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gsofddlot.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gzedptphm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gfvlzjtvf.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gxrzfnvbs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gmkgccgpz.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gsqmskwqx.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gcucniujw.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/guquxryuk.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gzjseebvy.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gkmkjqeoq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gmplzmsps.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gqrckusat.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gktqmtnga.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gforciemz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/glpfphngv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gmnbbohff.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gpaybqtdi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gcvsgsmdw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gigvqitbf.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/grtecumef.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gyrmfqowc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxulgqnpm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gbiruymyw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gknnshzwa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gzogwwemb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/guzuykffz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gxlifdurb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gbrbvtwfn.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gsgqujwcz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gayizffem.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gttsgomdb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gnyrncmbg.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gqnmybdzu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gblavcjef.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzqqgsria.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gagwrbtqx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gcomfnqvj.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gkcmsvlve.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gmodtdfbj.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gflzornak.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gcziihtec.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gpyrllybp.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/goswmcpof.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gvcxfhlke.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gcxeqawfj.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/geelwpzkc.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/ggpnsuggk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gifrtdpep.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gbyeeukfq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gwbtegeab.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gknfjqtsi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/guvfvujed.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gzzqqdvtd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gvicerlvr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gffefhfva.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gloafyjkd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gcgwhbekh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gxcdvrrnh.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gpcttccfo.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gsccborqt.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/grtgaxxrq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gsgrfgbab.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gcoifukxw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gypjdmaxy.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gwmzzeryk.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gkmyxnwam.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gyotcsutf.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gdhebffsv.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gtwqpccvu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/guhdfrfxr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gesnohswq.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gxiwbkrjb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gpogtliwp.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gwmhirgdq.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gfasrkbeh.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/giyyokczd.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gtuznsboo.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gyxcqjxsz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gkaetksxs.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/grynourtw.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gpaatbrym.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gbqqrnrvr.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gwqaiuves.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkolymmv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gxrepypbc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/glhwcydrg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/ggwkgvkfb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/ggtvvqhgk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gygwifsff.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gfnmuejmn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gkrikrind.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/ggbjfynii.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gxvvofxua.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gyimuvfdj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gbfozbftl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gkmvdhzdy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gruzkgblf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gjzvxyikw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/glabnlgia.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/glihdjwpf.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gvukwazti.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbednwueo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/godbrfhdj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gequezbba.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gvfeaaqcl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gmxvwptcd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gvyykizxa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gatjjzzij.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gqapjovca.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/ggjqibzeh.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gpmusxvlq.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gaddfovja.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gidastfna.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/geedqqjoa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gbsuautpa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/grlbqggvy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gerehygoy.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gbnelpdjz.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/grdpgskft.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gkvjdssge.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/glteiikdo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gjtrqgcee.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gcbqpgwja.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/giyvdwrdv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gauwnarkp.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gugfhqyuz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gowieyhsn.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gtrfgxver.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gdftauniq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gaztvgyam.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gyuuwhatd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gnoarowkb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gylyifgol.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gumiplrxo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/glryoqcup.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gxnwqyfbf.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gppjhnxsw.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gxhovojhg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gzyvjhgei.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/ghwayraal.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gntomtoyx.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gnvpmwfpu.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gsnowjwxb.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gpwfflmfl.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gcutkhizf.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/ghbnqqavp.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/glkoghtmp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gqtrghebq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gsppyrojj.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gyieukyhq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gpeswopcp.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gwtiucvyc.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/grhscwgbm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggxylffba.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gbtbucuqs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gzqauudpg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gzcjrvrvg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gclmvzejq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gndfbtgkg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/goqwnsvsc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/grlyipkug.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gdlfzddik.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gstjgeivd.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gkhoxqiic.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gvjrcwxay.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gngtkpjjd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/glusrdega.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gnbnufkfs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gsoeerdce.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gsrkfdobq.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gdkmkwqkp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gbcmlrwab.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkbznrrde.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gflhpwkza.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggvutyycs.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gwdajjukc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/grmpjycrv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ggbntxbht.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gubrvzibz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gjwpasixw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gbcnatlkn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/grmamawde.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvwhfkzen.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gayyeprvr.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gjwgohzfb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/grnijjazd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/ggqrlixca.sHtML


<!-- 参考信息 -->