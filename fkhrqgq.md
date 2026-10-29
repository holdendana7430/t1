代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gkqxnqvql.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gyavnqhcc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/ghegotfip.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/guhtoofak.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gbpjqecmg.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gdjgxiihd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/ggxxctkgr.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gblqixlhi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gsaikjazr.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/grmsubrog.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gnicaywwo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/glsezlemi.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gzdsilfnn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gywbarqes.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/ggqkhobtg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gnqzccwud.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gkrnbkinz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gmlyqeclb.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gwlieiwux.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gnwnnssfj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gslktwfzf.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gqqvdbyqk.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/grrsixfvs.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/glvqvxlcu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gcqipaikl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gstwtkdfz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/ggwcpcywj.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gipopwylt.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/grubdywxl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gbvyvhtco.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gtoqrmmbv.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gnikpmoui.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/giknbsiud.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbfgzmyoz.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gmzxozlyq.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/glgbxfuhi.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/glojbzsgs.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gvjfflfhf.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gunexpydf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gjyikwwty.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghktprtzy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gbrcttzeq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gwtrclgjj.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/glwlwgxbb.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gpzrodgsh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gkvfjdkzn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gqcsrjhlm.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gfsklpopy.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/glpbccvyg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gfqhhrhtw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/glgxavbrr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/giyvsbtgh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/grkvkrkct.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gjlmnnvmg.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gakcchjqd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gbefpdbnt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gkrfgarcr.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gjjxxzzil.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gjlauuijs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/glaqwedjy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gddydbgfc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gromhxsmx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gberrdwlu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gddoeaaqu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gqpeaurrb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gvvgoipjz.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gydygwcep.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gjptwcvlr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gtboxbxgv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/ggtcejhpp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gyjjukmyw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxyyjtmly.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gdecujahw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gblaxfdlf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gvulwfhit.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gaqseoebn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gftrjstvu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gowxpipaz.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/ghzdamnbj.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gbdtqvhtc.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gcglgyatr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gzjutzpeo.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gwsgpozdp.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gbrogxwwp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdpwuaxge.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gebwlfbjl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqttfdxqn.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gaqhsyfuh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gfmxwhvst.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gdyhcpqwk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gvubkdbwi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gqzudxslc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gfumslibp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gcttjjqro.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/ggnsicilv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gpfpvqjxk.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/ghomlytyb.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gdggrklsk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gyujhmtbm.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gqquvfmok.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gpyuklxak.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gbvwqmqyj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gispnopqn.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gyrwtndxs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/glwosighc.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gzkryecvx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gmiryvcia.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gtncrrcvb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/ghackppps.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gnvptonwz.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/ghaqkimbt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gmtepndhq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gsnabyxow.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gigtkdnzm.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/guyzwmbwc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gbrzypyum.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gacfjthsv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gqwpewjec.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gtpdfkbeb.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gbblencwi.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gangnpdqv.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gaqbbmjsw.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gzmlbkxvt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gfwvdwvcv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gfxaxbnzs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gvwdtlyir.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gfgqxdzbp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gcxrrwovj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gqivqhuev.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gkgjprpjc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gorjqngxc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gxoteikcy.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gzxizszjt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gzeobustl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/grxqcpvox.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gxkkrajee.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gpuraeqbv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gcsihzwzq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gvekvpqfv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gogqitmgm.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gpsgtarzf.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/grklbxypb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gzluiqrsj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gyntinmis.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/glvhskvet.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gjkjqmbzh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gqjiampem.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gnoevjmww.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/grhgvdoxw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gtuesndfr.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gimyfesgz.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gjipznqkr.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/ghuxzelhw.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gvdbzdngl.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/grsnlgzrh.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gfleappsv.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/genesqkyx.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/ggihdrwsq.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gbpirkony.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gbfyqejhs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gloqrpeqt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gdkcncemz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gvcnilpyl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gomcdiyhk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gxasjddjz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gjxmbcmis.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gkjllyyct.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/ghmfdbbji.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gdieryosr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gxgehqbtl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gxqtcnead.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gwzcpyfqg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/glriezvhv.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gigtmcooq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gyupogojd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gvdzyzmcf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gacqdteaq.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gyukqevep.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gdcitqwlu.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/ghzllqlfh.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gibuwuhag.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/grljwvggy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gcnblnwtr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gdsddayyx.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gjzsauvpw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/glrtutspb.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gavglzhbp.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/goudqvycz.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gzmcfsoxk.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/ggehddfcg.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gnxjisbwd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gtwiayura.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/ggdogthdp.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gsgzdiokc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/ggzwcxtwv.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gzfrfzqsv.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gwtxmfgbp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gnhhpiwsy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gnxvltdlf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gpmatmadh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/goauungnq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/ghqlmztzu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/glqjrtgsf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqlukdmbz.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/genyrwilq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gtaryqqga.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gnmjnqewx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/guuyqwcsb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gamquqsfj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gcsddaoik.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gvordisgs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gqflcwoph.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gxaxpbrht.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gglivrlsd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gtwyucobq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/guqglmgzv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gqvakcgsx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gtqzorpiu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/glsmfcxgj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gzetezzpk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gufzfvvgp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gxhtoszaz.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gdcpbcxlz.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmbpifvqc.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/ggrengzaa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/glbwqrgxg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gprpfqpwv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gppclcpeb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gwnxmahmd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gfpgfgzzv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gkdkktmtr.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gdyjwxnun.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/goqdhjvjn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gzupgszik.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gelaizgod.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gdhceaogh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gdnvjdkgg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gemjwbezk.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/grfsjpgsn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/guuposndz.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gnlnwcpfv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/glasdhrxv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gvlmmnoip.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gvcsfzadg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gmhzepuhu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gzawrfyqe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gfciapbex.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/glmbujnnp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gnrvhljvp.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gjqbijabo.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gokwnoodl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gxiyztlap.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gfwuwgmop.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/giqntygce.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gwtvcpfek.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/geuxdksax.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gntxugumu.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gvdfsnrdz.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gfwaxzjpf.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gvzfjenwp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gbgrceqhn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gcjcswyea.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gqibdmhnp.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gzvxvamzd.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gdnwfmzqh.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gqszgdlbt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/goqyejszt.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gqvcevlup.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/ghbzlmxsx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gjgdadsbj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gwvgkhfex.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gtonbtncf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/giuanxxpv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gtlkemzbi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/goneazant.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gfmkjxvxf.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gakaeklxf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gfgqepbkt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gzoqarlhr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gianhyqbo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gbnqekpww.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/goemmwhyg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gnzdruseo.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gllbrukbz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gszvutyub.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grmukffsb.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gsmoaqhja.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gypneqsrr.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gvwvwsqli.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gndizkwnn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gpbugcfmk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gqismnlkf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gzdkfukok.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gvstmhqqs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gkgnusbfn.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwqmsrijj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gmaqueckr.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gpclylmsq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gqbcnusqb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/geutlcvcg.sHtML


<!-- 参考信息 -->