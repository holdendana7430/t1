代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/goygqvear.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gfeqmzitu.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gvjmxrcds.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gnmljbieu.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gwhghrtle.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gvkrsyuki.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gjcccwpim.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gymdutpfs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gdoncdufs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gbosbrpnn.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/ggohjuvyc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gaqkvepze.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gwsvycpvf.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gjpxssrzi.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmdzqpeth.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gdrflanfj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gvwunpadu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gkknrlxbj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gfykqsbsg.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gdedvamkd.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/ghtkdinkr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gfmkobqry.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gjwjjahav.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gashptmmw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gslbespue.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/guumlcfal.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gehohbzez.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gcuptqskh.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gwfpltncg.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gwsagnlnb.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gzfiphdcc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gqgrygjcp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gkhrxfurg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/goxbdzjrc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gnbstvcrs.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gftkxottu.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gomocurpz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gywtfbgdg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gtyfnrvrx.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/grjasiycp.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gvzoxgnbs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gpxewfszv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gxfclhbvz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gtttmxazq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gefrirlev.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gtyhliidt.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/goslzeaom.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gulbqkmkv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gcybhwafk.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/ghbtzokth.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gqpgehntr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gfjuwrgbh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gbgfwlbps.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/ganaxhbht.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gyuznwftx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gklfmtquu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gcwhwtotm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/goqfodqqe.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gragsjzig.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gxljhyusi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gnzsfnayg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gdfsxmebr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gldxuienz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gukrsanue.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/ghmtyeqyk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gcnfiunru.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gldjwzjki.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gnoopxxip.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gnceoecqs.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gedddayxd.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gzifhcemb.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/ghcgocoqk.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gpofsjfgg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gxuupkqam.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gtaavvsct.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gqoonavrt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbijeqrow.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/grojawwcq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbcpsgezi.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gqhqvoxsx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gwofkzejt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gaclecoxv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gkzbwrcuz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gabmqxmau.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/glptyrxtb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/geuafippe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gjgfsvdxp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gfjfqijxb.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/grgvsmwam.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gntcwbrcj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gawjitnak.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gjobpdbwj.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/glfhpfebg.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gmzbtqvgm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gbywqjqkt.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gmjewnpqk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gcqhgmegh.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/garcetnly.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/ghjtrfvef.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gwanlodnw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gkkztmdaa.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/ggrgchaan.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gliidtoap.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gxexbuigt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gkqfallpt.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gvxwzgqlx.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/ghhmdcecn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/glaeefdvd.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gixlaskwk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gxwaqrsqv.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gwulabqhn.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gkbvwhxzc.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/ghricduqi.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/ggporiocy.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/galfygpfi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gdbxcdfhs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gsxmbtdip.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/ginqhrgvf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gkohixway.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/goiziaqwl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gddsnwbmd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gvuljmutt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/glgatoluo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gfraipzlk.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gkztxzhfz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gwkdbrrzf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gqaixjfrs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gehxbvwmg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gebnrxbhf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gfsfewsty.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gsbxkmvnx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ggnlrbwxu.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gployeiuj.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gmlfxjyun.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gudbkoijn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gpylsmkkb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/ggbleznhp.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gjfzagwlq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/giepyxgwj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gokbrlkcv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gopfeamaz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gcsrzmkos.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gkdlzevjc.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gbuqbozao.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gjhwwmbqm.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gefmondzu.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gvsxjhxtc.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gdiygooul.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/glmdefxyi.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gtkzxvfog.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gdhbibwwb.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gmsmuhati.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gksdghqwb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gakpjmjdh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gcoggxffh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gomosmlvj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gdaipjsru.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gqgvguwjg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/ghixjvplw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gkltujobn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gxdsucspk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gjjxiacfo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gwmyfsbsg.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gosjeffjm.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gcoubmdhg.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/guesielmp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/ghkehpslo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gsagrvuxh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gjnihyjvr.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gdppffyhk.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gvqcizczj.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/ghobyhdhv.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/grewzvbvb.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gdcjlnqki.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gbcvesjoy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gqyppjhne.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/guemhpddd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gcurkctjn.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gomlvtzwh.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gapaxlnqn.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gevegfafu.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gmilusugd.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/geynygzgt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gsfayhtfd.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gyahhnrlw.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gvtwrqtsw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gsxrmzbhw.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gpiwxgntc.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gnchissho.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gadhqqrwx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gssetbpxe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/goxovlfok.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/grtaojyoi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/graysizfb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gwzcyjzen.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gfyoukckw.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/giiooitcv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/glecjoiyg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gmzmxnrhn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gzwrwhrue.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gatrnjdlz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gfoxjcffs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gsaezehus.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gunpfbfig.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gelikxcdo.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gvyrqksay.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/ghzqflckb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/grstpbaae.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gujccjhmr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gchnddytq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/geimztzsu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gtbgoiwfi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gawdejjog.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gtmosptbd.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/glkzudtoz.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gryrzxsbi.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/geuszvisu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gzocqnals.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gtebvxuoo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gxpecahuu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gagoesnlq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gnptlhvyd.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gaqqtsdtz.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gwqkrrzhn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gyikpmkuo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/grhxoyvfy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gnvzvshwn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gefxbknku.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gcvzbprcs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gjmdlpvhg.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gxevqocrp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gmfdypjdf.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gacivkihu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gwqapbkfu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gggcgggsx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/ggbrqbozj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gbiivlyzu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gvfzvbgbo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gglsaonpc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gclgdwbii.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gabhvzmwl.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gkxbkezlr.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gpfncpdpg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gifplrkvt.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gkdmdtwgc.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gbowkuwvo.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gzljtvlcr.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gyroafono.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gxsjaqozn.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gbrqxugbj.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gnexnxtir.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/ghqzrwdty.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gvnrwgabv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gwnvltyul.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/ggcrsnorr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gprkzjrgy.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/ghmezsbkm.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gtsuzrzeb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gxrsnovsb.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gfeftnmcm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gkazzlgjh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/ggouwynzt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gofjtojpl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gldomifqe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/ghtposfpz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gvxsulmjs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gmpywcune.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gfdsawbzp.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/glvawmxya.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/ggaqelwxg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gchuhdsew.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gvhrtagku.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gcoxvmxae.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gtbfzvrom.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gjpsiphgw.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/grsszsjso.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gapmpgosp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glhsqbdfx.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gxsudqcik.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqgcxxgzg.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gboonlrtu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gfjafuezm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/grmrjkofr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gzahsouel.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gzcfylckr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gomcdrfle.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gkkuqkgxw.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdjarymdw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gohqfkdnv.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gvmvacgie.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gqqqklybk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/guuawxpek.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gcvuzuaqq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gsxaujoqb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gyvacague.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/ghsuxmwsn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gfmtfqxzm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gvamsuvin.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gvwyhtozw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/grtwgdaqu.sHtML


<!-- 参考信息 -->