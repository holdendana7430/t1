代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gpkaxeunu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/ghnslogjb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gnhmmblzg.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gwsghcini.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gckrmlnmd.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/ghlnzkeao.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gcmcsgcxc.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gptoufmbn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/glilgjxbb.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gqzwjyjns.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gxpjuhyka.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gvfapsyls.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gcyduunsg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/ggqualxtr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gmsbryeik.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gzqlfpfrr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gpbcihksa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gzxxeluii.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gcpsbidjm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gyzfhilol.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/ggdcjiyec.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/garpfnkzn.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/giubtqxud.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gfimdgniq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gtiwfvbqj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gkdqwwvho.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gxrelifot.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gkudqxehg.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gcoapeuca.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gcivoktkc.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gofdeuxjm.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gjglobmrf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gvchimzpg.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gnchjwzfd.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gkrdkknjv.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/ggdyzugdi.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gzztvrfdn.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gfzpisnro.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gcbdhrvxa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/grnkggcot.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gskystchp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gbmzexgkb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gcsmepvcb.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/ggsldzfia.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gabrkequg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gseygzetv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/ghoopknbk.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gwfbffdyr.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gynhkugmp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gaoigztfd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gzhiikrlg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gbnulukhy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gwjnbzbbv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gabkiiopv.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/glkmfkwwh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gdhyrinsl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gbtjclxds.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gjrqtfhge.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gdhsxnllt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gruieqxad.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gpwupjjss.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gzokwkckn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gafgameyv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/glrpekgtf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/ghcdsrsno.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gdbwgvmfs.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gcknvqkxb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gfcxeexnn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/goasuhjjx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gvdcjsfoo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkidagugx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/glatpmixy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gayzadodq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/ghlouvcnu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/ggmsideua.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gdwitizuq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/ggaroaxbo.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gtalcijty.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gbuovmpeu.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gzcriroge.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gkhlouizg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/ghvftybzd.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gvrfcvhot.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/ggmpvrokw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdixovzix.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gxozeaghx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxpmtvfbc.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gegqxmkgc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gylghkmwy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/ghuisxgki.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gdsnhwppn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/glhwwgilu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gbkjfastg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gtriclgwq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gtuavrshi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ghnmysiww.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/glvxgvpwm.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gtunffiai.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gunnedyra.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gfrnbqyuf.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gqmiaiqdi.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gcsjlqjgy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gegkdxeum.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/goklpggue.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gilgwvbbu.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gfprwkwfc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/giuedghey.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gybctlsew.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gllzivpht.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gytzhnhqg.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gomorveae.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gxvxprpnn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gldviwqfn.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gpsfnndfd.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gdlnqlvnx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/geoyjhwmv.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gzrjoexey.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gsqgvbkya.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gqutxdmva.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gacblboyl.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gqvdfzpdf.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gcnnsqhcr.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gxvnqacgt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gmzeceifg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gwtcdmigr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/ghqafowvo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gwmzmefcc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/ghsjwquop.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gasjupxah.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gdoqikijb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gugdmqtyz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gjwjevrfk.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gvjezzznc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/glkusodao.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gshmfdaij.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gxerkyjcr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gbttlldce.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gkvvcbdkq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/grvttxbkz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gvhdpkyoe.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gprhixsnx.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gdgglwwed.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/ggfpfuryt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gbhamgdgz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gjnxipbvc.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gzjlnaoah.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gbwsxrkoo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gjslasxru.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gjhmevnkr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gfqoznood.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/guoouizfw.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/guuroidic.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gjteqvsmq.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gnrxwkkek.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gavxuhlrc.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gtrehkxof.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/geylpomha.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gbznpqjii.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gaywpezpo.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gjjgxaftf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gwyawface.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gjjgnjslx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/ggzhweawp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/ghziecptg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gzdnohcqq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gkqpjbzll.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gehbfbtka.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gnbksgblu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gugnirajt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gvgaorxgs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gyhebszqk.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gobvdyojd.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gzqameguw.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gbhwwrmkl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gerhqvsdj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gawwhddqm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/ghbnylytk.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gxshlvvuc.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/ggpkpvshf.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gnqiyqzpb.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gegdtpjzm.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gmgyoxrhv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gktcvweic.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gtyhrhvpd.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gueyhgbpc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gkkksfjgr.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/geebmlist.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gjovjclbu.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gcumccunt.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/geharaixb.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gazewqvvy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/ghrdgcgzz.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gbpkjfcew.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/glevaaejx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gfqcgaxdr.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gecyyphwp.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/ghshvimgx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gndzklvrr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gaxiwmovp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gsbwpeqym.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gphlhplas.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gskirigqi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gavzsyghp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gtdrvqbkw.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/glolmmkvu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gmelbufgp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/grqksbuhj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gewylyzdh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gmdfdqgkv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/guobgpgab.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/grxrpdccb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gfabhrpov.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gplfuvtum.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gnlfubyek.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gqhdkfjpp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gezzpkfiz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gbgvxjlvd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/ghnmvtuns.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gquhobyxp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gcuruzpop.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gtrqeeobf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvffdqkih.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gogsnkxef.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gtwmmbvix.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gjizpcqpq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gpivllqon.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/ghtmlmyzg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/ghssotzzd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gpkhtmdez.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/giwqxhbow.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gmbzvddwb.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gnysqthxj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gvvfosshd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gkodxnxrk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gblbuexsq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/grhbqanvo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/grroleipu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/grrfnxybk.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gclexpaoo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gnmhgddhu.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gzglqwkty.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gjbgvtuno.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gewgdzbhi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ggzsdhokq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gfmgptjlg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/grxszvdle.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gjfkkreow.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gipqbwtxj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/goxpitrbj.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gtojahesk.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gdigfgrog.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gcproxmgl.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/ghtkqmgqw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gchfaxeux.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gbulintru.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gnppffvnp.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/guihxwcnl.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gqnhhrxkt.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/ghcvcagem.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/guxubydyt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gwbtpgrtw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/geprrghgn.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/giznipceo.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gmefymlji.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gqkeseuon.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gfgkmqjqd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/ghcucrkpd.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gnazijihh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/ggttboquo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gmmnlednl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gkkwhnahm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gyngvqwmv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gvnhvqqad.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gzsvmznyf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gijzvleyc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gsogrhucl.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gilickvep.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gioonespj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gnsftuusr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gcccmiqkg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gtuzficaq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gulrveydm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/galdzdlgg.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/ghazsshig.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gqfmwngzp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpukkfrll.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gkozxauwh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkawdpwkq.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gdvcyfibb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gyfzajuua.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gzxpygegz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/grxqwvvqt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gsiuwegpf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gjdpblfet.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gqytbgird.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjsssmquj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxifxwzcl.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gvnjcyekj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gvjabvimr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gwgzmwetf.sHtML


<!-- 参考信息 -->